<script>
  export let classes = {};
  $: contentClass = classes.content || "";
  $: headerClass = classes.header || "";
  $: footerClass = classes.footer || "";
</script>

<div class="min-h-screen flex flex-col">
  <div class={headerClass}>
    <slot name="header" />
  </div>
  <div class="{contentClass} flex-1">
    <slot name="content" />
  </div>
  <div class={footerClass}>
    <slot name="footer" />
  </div>
</div>
