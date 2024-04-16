<script>
  //import { onMount } from 'svelte'//현재 컴포넌트가 준비되면 콜백 함수의 내용을 실행하겠다
  import svelteLogo from './assets/svelte.svg'
  import viteLogo from '/vite.svg'
  import Counter from './lib/Counter.svelte'
  let text = "";
</script>

<main>
    <h1>{text}</h1>
    <input type="text" 
           value={text} 
           on:input={(e) => {text = e.target.value}}/>
    <button on:click={() => {text = 'Heropy'}}>Click</button>
</main>
