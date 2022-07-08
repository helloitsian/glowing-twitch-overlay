<script>
</script>

<div class="Camera__camera">
  <div class="Camera__shadow"></div>
  <div class="Camera__border"></div>
  <div class="Camera__section"></div>
  <div class="Camera__details">
    <div class="Camera__details-title">
      <h3>StreamingLotus</h3>
    </div>
  </div>
</div>

<style>
  @keyframes glowingMovingGradient {
    0% {
		  filter: blur(.3rem);
      background-position: 0% 50%;
    }
    50% {
      filter: blur(.5rem);
      background-position: 100% 50%;
    }
    100% {
      filter: blur(.7rem);
      background-position: 0% 50%;
    }
  }

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

  .Camera__shadow {
    position: absolute;
    top: var(--top, 20px);
    left: calc(var(--left, 1) - 5px);
    right: calc(var(--right, 1) - 5px);
    width: calc(var(--width, 569px) + 6px);
    height: calc(var(--height, 569px) + 6px);
    z-index: 2;
    border-radius: 25px;
    background: linear-gradient(-45deg, #ee7752, #e73c7e, #23a6d5, #23d5ab);
    background-size: 200% 200%;
    filter: blur(.3rem);
    animation: glowingMovingGradient 10s ease infinite alternate-reverse;
  }

  .Camera__border {
    position: absolute;
    top: 20px;
    left: var(--left, 1);
    right: var(--right, 1);
    width: var(--width, 569px);
    height: var(--height, 330px);
    z-index: 2;
    border-radius: 25px;
    background: linear-gradient(-45deg, #ee7752, #e73c7e, #23a6d5, #23d5ab);
    background-size: 200% 200%;
    background-position: 0% 0%;
    animation: movingGradient 10s ease infinite alternate-reverse;
  }

  .Camera__section {
    position: absolute;
    background: #04ff00ff;
    top: calc(var(--top, 20px) + 12px);
    left: calc(var(--left, 1) + 11px);
    right: calc(var(--right, 1) + 11px);
    width: calc(var(--width, 569px) - 24px);
    height: calc(var(--height, 330px) - 24px);
    z-index: 3;
    border-radius: 20px;
  }

  .Camera__details {
    position: absolute;
    top: calc(var(--height, 330px));
    left: calc(var(--left, 1));
    right: calc(var(--right, 1));
    width: calc(var(--width, 569px));
    text-align: center;
    z-index: 3;
  }

  .Camera__details-title {
    color: white;
    font-size: 1.5rem;
    margin: 0;
  }
</style>