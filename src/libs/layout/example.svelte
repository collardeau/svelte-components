<script>
  import Layout from "./index.svelte";

  let classes = {
    header: "h-12",
    content: "bg-gray-200",
    footer: "bg-gray-400"
  };
</script>

<Layout {classes}>
  <header slot="header">My Header</header>
  <section slot="content">My Content</section>
  <aside slot="left">Left Section</aside>
  <aside slot="right">Right Section</aside>
  <footer slot="footer">My Footer</footer>
</Layout>
