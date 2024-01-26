<script>
  let count = 0;
  function increament() {
    count++
  }
</script>

<button on:click={increament}>
  Click {count}
</button>


<style>
  button {
    padding: 15px 20px 15px 20px;
    border-radius: 10px;
    border-color: blue;
  }
</style>