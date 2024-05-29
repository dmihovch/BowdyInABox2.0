<script>
  let clicks = 0;
  function onClick() {
    clicks++;
    console.log(clicks);
    if (clicks < 5) {
      //shake
    }
    if (clicks === 5) {
      //explode
      clicks = 0;
    }
  }
</script>

<button class="shake" on:click={onClick}> Hello World </button>

<style>
  .shake {
    background-color: red;
  }
  .explode {
    display: none;
  }
</style>
