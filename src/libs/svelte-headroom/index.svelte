<script>
  import { createEventDispatcher } from "svelte";
  import validate from "./validation";

  export let duration = "300ms";
  export let offset = 0;
  export let tolerance = 0;

  let headerClass = "";
  let lastHeaderClass = "";
  let y = 0;
  let lastY = 0;
  let prefix = "svelte-headroom--";

  const dispatch = createEventDispatcher();

  function deriveClass(y = 0, scrolled = 0) {
    if (y < offset) return "";
    if (Math.abs(scrolled) < tolerance) return headerClass;
    if (scrolled > 0) return "";
    if (scrolled < 0) return `${prefix}unpin`;
    return headerClass;
  }

  function updateClass(y = 0) {
    const scrolledPxs = lastY - y;
    const result = deriveClass(y, scrolledPxs);
    lastY = y;
    return result;
  }

  function action(node) {
    node.style.transitionDuration = duration;
  }

  $: {
    validate({ duration, offset, tolerance });
    headerClass = updateClass(y);
    if (headerClass !== lastHeaderClass) {
      dispatch(headerClass ? "unpin" : "pin");
    }
    lastHeaderClass = headerClass;
  }
</script>

<style>
  div {
    position: fixed;
    width: 100%;
    top: 0;
    transition: transform 300ms linear;
    transform: translateY(0%);
  }

  .svelte-headroom--unpin {
    transform: translateY(-100%);
  }
</style>

<svelte:window bind:scrollY={y} />
<div use:action class={headerClass}>
  <slot />
</div>
