<script>
  import Counter from "./lib/Counter.svelte";
  import Button from "./lib/Button.svelte";

  let name = "Svelte"
</script>

<Counter />
<Button size='large' shadow>Something interesting</Button>

<h1>You are welcome to the 
  <u>
    <strong>{name}</strong>
  </u> Tutorial.
</h1>

<style>
 strong {
  color: rgb(244, 47, 3)
 }
</style>