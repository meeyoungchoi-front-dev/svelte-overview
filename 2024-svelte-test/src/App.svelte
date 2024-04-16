<script>
  import svelteLogo from './assets/svelte.svg'
  import viteLogo from '/vite.svg'
  import Counter from './lib/Counter.svelte'
  let name = 'world';
  let toggle = false;
  if (toggle) {

  } else {

  }
</script>

<main>

<button on:click={() => {toggle = !toggle}}>Toggle</button>
{#if toggle}
  <h1>Hello {name}</h1>
{:else}
  <div>
    No Name!
  </div>
{/if}
</main>

<style>
  h1 {
    color: red;
  }

  .active {
    color: blue;
  }
</style>
