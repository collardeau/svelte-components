<script>
  import Header from "./index.svelte";

  let toggleDrawer;
  const handleClick = () => {
    toggleDrawer();
  };
</script>

<style>
  :global(.fluid-header-container) {
    background-color: lightblue;
    padding: 10px;
  }
  :global(.fluid-header-button:hover) {
    font-weight: bold;
  }
</style>

<Header
  as="header"
  breakpoint="md"
  duration={250}
  bind:toggleDrawer
  on:open={() => {}}
  on:close={() => {}}>
  <div slot="left">
    <h1>My app</h1>
  </div>
  <div slot="right">My Horizontal Menu</div>
  <div slot="drawer">My Vertical Menu</div>
  <div slot="right-collapsed">
    <button on:click={handleClick}>Toggle</button>
  </div>
</Header>
