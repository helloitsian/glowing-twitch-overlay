<script>
  import Socials from '../components/Socials.svelte'
</script>

<main class="Brb">
  <div class="Brb-wrapper">
  <span class="Brb__title gradient-text">
    Brb...
  </span>
</div>
<Socials />
</main>

<style>
   @keyframes movingGradient {
    0% {
		  background-position: 0% 50%;
    }
    50% {
      background-position: 100% 50%;
    }
    100% {
      background-position: 0% 50%;
    }
  }

  .gradient-text {
    color: transparent;
    background: linear-gradient(-45deg, #ee7752, #e73c7e, #23a6d5, #23d5ab);
    -webkit-background-clip: text;
    background-size: 200% 200%;
    background-clip: text;
    animation: movingGradient 10s ease infinite alternate;
  }

  .Brb {
    width: 100vw;
    height: 100vh;
    background: black;
  }

  .Brb__title {
    margin: 0;
    font-weight: bold;
    position: absolute;
    font-size: 35em;
    top: 50%;
    transform: translateY(-50%);
  }
</style>