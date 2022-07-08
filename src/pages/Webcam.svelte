<script>
  import Socials from '../components/Socials.svelte'
  import Camera from '../components/Camera.svelte';
  import Chat from '../components/Chat.svelte';
</script>

<main class="Webcam">
  <div class="Webcam__cam-chat-wrapper">
    <Camera --top={"20px"} --left={"20px"} --width={"1300px"} --height={"731px"}/>
    <Chat --width={"566px"} --height={"1040px"} --bottom={"20px"} --right={"20px"} />
  </div>
  <Socials />
</main>

<style>
  .Webcam {
    background: url('https://w.wallhaven.cc/full/3z/wallhaven-3zgyzv.png');
    height: 100vh;
  }
</style>