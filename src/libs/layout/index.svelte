<script>
  export let breakpoint = "sm";
</script>

<style>
  .collapsible:empty {
    flex: 0;
  }
</style>

<div class="svelte-layout-small min-h-screen flex flex-col {breakpoint}:hidden">
  <slot name="header" />
  <slot name="menu" />
  <div class="flex-1">
    <slot name="main" />
  </div>
  <slot name="aside" />
  <slot name="footer" />
</div>

<div class="svelte-layout-large min-h-screen flex-col hidden {breakpoint}:flex">
  <slot name="header" />
  <div class="flex-1 flex">
    <div class="flex-1 collapsible">
      <slot name="menu" />
    </div>
    <slot name="main" />
    <div class="flex-1 collapsible">
      <slot name="aside" />
    </div>
  </div>
  <slot name="footer" />
</div>
