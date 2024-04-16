<script>
  import svelteLogo from './assets/svelte.svg'
  import viteLogo from '/vite.svg'
  import Counter from './lib/Counter.svelte'
  let name = 'world';
  let age = 85;
  function assign() {
    name = "코딩묭이";
    age = 29;
  }
</script>

<main>
<h1>Hello {name}</h1>
<h2 class={age < 85 ? "active": ""}> <!--중괄호를 이용한 선언적 랜더링을 사용할 수 있다-->
  {age}
</h2>
<img src="" alt={name}/>
<input type="text" bind:value={name}/> <!-- bind를 활용하여 name 필드에 데이터를 바인딩해줄수 있다-->
<button on:click={assign}>
  Submit
</button>
</main>

<style>
  h1 {
    color: red;
  }

  .active {
    color: blue;
  }
</style>
