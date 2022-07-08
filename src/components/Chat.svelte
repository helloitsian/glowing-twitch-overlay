<script>
  export let top;
  export let right;
  export let width;
  export let height;
</script>

<div class="Chat" style="">
  <div class="Chat__title">
    Chat
  </div>
</div>

<style>
  .Chat {
    display: flex;
    justify-content: center;
    position: absolute;
    width: var(--width, 566px);
    height: var(--height, 650px);
    bottom: var(--bottom, 20px);
    right: var(--right, 20px);
    border: 1px solid black;
    border-radius: 25px;
    background: rgb(0, 0, 0, .3);
  }

  .Chat__title {
    font-size: 2rem;
    font-weight: bold;
    color: white;
  }
</style>