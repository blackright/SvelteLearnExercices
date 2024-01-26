<script>
  let count = 0;
  let count2 = 0
  let string;

  function setCount2(x) {
    count2 = x;
  }

  function increament() {
    count++
  }

  $: setCount2(count)
  $: string = `The Variable Count2 is ${count2}`
</script>

<button on:click={increament}>Click {count}</button>
<h3>{string}</h3>

<style>
  button {
    padding: 15px 20px 15px 20px;
    border-radius: 10px;
    border-color: blue;
  }
</style>