<script>
  import Layout from "./index.svelte";
</script>

<style>
  /* target size specific styles: */

  :global(.svelte-fluid-layout-large main) {
    width: 66%;
  }
  :global(.svelte-fluid-layout-small section) {
    padding: 10px 0;
  }

  /* your app styles: */

  :global(body) {
    margin: 0; /* reset */
  }

  header,
  footer {
    background-color: lightblue;
    height: 60px;
  }
  section,
  aside {
    background-color: lightslategray;
  }
</style>

<Layout breakpoint="md">
  <header slot="header">Header</header>
  <section slot="side1">Side 1</section>
  <main slot="main">Main</main>
  <aside slot="side2">Side 2</aside>
  <footer slot="footer">Footer</footer>
</Layout>
