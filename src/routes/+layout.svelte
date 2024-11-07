<script>
  import Nav from "./common/Nav.svelte";
  import Contact from "./common/Contact.svelte";
  import Follow from "./common/Follow.svelte";
  import "../app.css"

  let { children } = $props();
</script>

<div id="app">
  <Nav/>
  <main> {@render children()} </main>
  <Contact/>
  <Follow/>
</div>