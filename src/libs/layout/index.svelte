<script>
  export let classes = {};
</script>

<div class="min-h-screen flex flex-col">
  <slot name="header" />
  <div class="flex-1 flex">
    <div class="flex-1">
      <slot name="menu" />
    </div>
    <slot name="content" />
    <div class="flex-1">
      <slot name="aside" />
    </div>
  </div>
  <slot name="footer" />
</div>
