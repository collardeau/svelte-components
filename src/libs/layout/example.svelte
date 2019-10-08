<script>
  import Layout from "./index.svelte";
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
    width: 66%;
  }
  section {
    background-color: burlywood;
    min-height: 100%;
  }
  aside {
    background-color: lightseagreen;
    min-height: 100%;
  }
</style>

<Layout>
  <header slot="header">Header</header>
  <main slot="content">Content</main>
  <section slot="menu">Menu</section>
  <aside slot="aside">Aside</aside>
  <footer slot="footer">Footer</footer>
</Layout>
