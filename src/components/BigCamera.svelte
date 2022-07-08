<script>
</script>

<div class="BigCamera__camera">
  <div class="BigCamera__shadow"></div>
  <div class="BigCamera__border"></div>
  <div class="BigCamera__section"></div>
  <div class="BigCamera__details">
    <div class="BigCamera__details-title">
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

  .BigCamera__shadow {
    position: absolute;
    top: 20px;
    right: 15px;
    width: 575px;
    height: 336px;
    z-index: 2;
    border-radius: 25px;
    background: linear-gradient(-45deg, #ee7752, #e73c7e, #23a6d5, #23d5ab);
    background-size: 200% 200%;
    filter: blur(.3rem);
    animation: glowingMovingGradient 10s ease infinite alternate-reverse;
  }

  .BigCamera__border {
    position: absolute;
    top: 20px;
    right: 20px;
    width: 569px;
    height: 330px;
    z-index: 2;
    border-radius: 25px;
    background: linear-gradient(-45deg, #ee7752, #e73c7e, #23a6d5, #23d5ab);
    background-size: 200% 200%;
    background-position: 0% 0%;
    animation: movingGradient 10s ease infinite alternate-reverse;
  }

  .BigCamera__section {
    position: absolute;
    background: #04ff00ff;
    top: 31px;
    right: 31px;
    width: 545px;
    height: 309px;
    z-index: 3;
    border-radius: 20px;
  }

  .BigCamera__details {
    position: absolute;
    top: 330px;
    right: 20px;
    width: 569px;
    text-align: center;
    z-index: 3;
  }

  .BigCamera__details-title {
    color: white;
    font-size: 1.5rem;
    margin: 0;
  }
</style>