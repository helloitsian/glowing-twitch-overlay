<script>
  import { Router, Route } from "svelte-routing"
  import Home from './pages/Home.svelte'
  import Webcam from './pages/Webcam.svelte'
  import Brb from './pages/Brb.svelte'


  export let url = "";
</script>

<main class="App">
  <Router url="{url}">
    <Route path="/brb"><Brb /></Route>
    <Route path="/"><Home /></Route>
  </Router>
</main>

<style>
  @import url('https://fonts.googleapis.com/css2?family=Fira+Code:wght@300;400;500;600;700&display=swap');

  :global(*) {
    font-family: 'Fira Code', monospace;
    box-sizing: border-box;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
  }

  :global(html), :global(body) {
    margin: 0;
    padding: 0;
  }
</style>