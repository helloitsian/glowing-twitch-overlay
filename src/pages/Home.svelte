<script>
  import Camera from '../components/Camera.svelte'
  import Chat from '../components/Chat.svelte'
  import Socials from '../components/Socials.svelte'
</script>

<main class="Home">
  <Camera --top={"20px"} --right={"20px"} --width={"569px"} --height={"330px"}/>
  <Chat --width={"566px"} --height={"650px"} --bottom={"20px"} --right={"20px"} />
  <Socials />
</main>

<style></style>