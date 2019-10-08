<script>
  import Layout from "./index.svelte";

  let breakpoint = "md";
</script>

<style>
  header {
    height: 60px;
    background-color: lightblue;
  }
  footer {
    height: 60px;
    background-color: lightpink;
  }
  main {
    background-color: white;
  }
  section {
    background-color: burlywood;
  }
  aside {
    background-color: lightseagreen;
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
  :global(.svelte-layout-large section) {
    min-height: 100%;
  }
  :global(.svelte-layout-large aside) {
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
