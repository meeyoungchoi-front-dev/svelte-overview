<script>
  import svelteLogo from './assets/svelte.svg'
  import viteLogo from '/vite.svg'
  import Counter from './lib/Counter.svelte'
  let name = 'world';
  let fruits = ['Apple', 'Banana', 'Cherry', 'Orange', 'Mango'];
  function deleteFruit() {
    fruits = fruits.slice(1);
  }
</script>

<main>
<h1>Hello {name}</h1>
<ul>
    {#each fruits as fruit}
      <li>{fruit}</li>
    {/each}
</ul>
<button on:click={deleteFruit}>Eat it!</button>
</main>

<style>
  h1 {
    color: red;
  }

  .active {
    color: blue;
  }
</style>
