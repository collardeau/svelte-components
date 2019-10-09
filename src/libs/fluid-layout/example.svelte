<script>
  import Layout from "./index.svelte";

  let breakpoint = "md";
</script>

<style>
  header,
  footer {
    height: 60px;
    background-color: lightblue;
  }
  section,
  aside {
    background-color: lightslategray;
  }

  :global(.svelte-layout-small section) {
    height: 100px;
  }
  :global(.svelte-layout-small aside) {
    height: 50px;
  }

  :global(.svelte-layout-large main) {
    width: 66%;
  }
  :global(.svelte-layout-large section, .svelte-layout-large aside) {
    min-height: 100%;
  }
</style>

<Layout {breakpoint}>
  <header slot="header">Header</header>
  <section slot="menu">Menu</section>
  <main slot="main">Content</main>
  <aside slot="aside">Aside</aside>
  <footer slot="footer">Footer</footer>
</Layout>
