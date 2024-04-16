<script>
  import { onMount } from 'svelte'//현재 컴포넌트가 준비되면 콜백 함수의 내용을 실행하겠다
  import svelteLogo from './assets/svelte.svg'
  import viteLogo from '/vite.svg'
  import Counter from './lib/Counter.svelte'
  let name = 'world';
  let isRed = false;
  onMount(() => {
    const box = document.querySelector(".box");
    box.addEventListener('click', () => {
      isRed = !isRed;
    })
  })
  
</script>

<main>
<h1>Hello {name}</h1>
<div class="box" style="background-color: {isRed ? 'red' : 'orange'}">Box!</div>
</main>

<style>
  .box {
    width: 300px;
    height: 150px;
    background-color: orange;
  }
</style>
