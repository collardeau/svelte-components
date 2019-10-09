<script>
  import Layout from "./index.svelte";

  let breakpoint = "lg";
</script>

<style>
  :global(body) {
    margin: 0;
  }

  header,
  footer {
    height: 60px;
    background-color: lightblue;
  }
  section,
  aside {
    background-color: lightslategray;
  }

  :global(.fluid-layout-small section) {
    height: 100px;
  }
  :global(.fluid-layout-small aside) {
    height: 50px;
  }

  :global(.fluid-layout-large main) {
    width: 66%;
  }
  :global(.fluid-layout-large section, .fluid-layout-large aside) {
    min-height: 100%;
  }

  :global(.flex-1) {
    background-color: pink;
  }
</style>

<Layout {breakpoint}>
  <header slot="header">Header</header>
  <section slot="menu">Menu</section>
  <main slot="main">Content</main>
  <aside slot="aside">Aside</aside>
  <footer slot="footer">Footer</footer>
</Layout>
