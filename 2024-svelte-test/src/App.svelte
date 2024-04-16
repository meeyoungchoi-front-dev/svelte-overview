<script>
  import svelteLogo from './assets/svelte.svg'
  import viteLogo from '/vite.svg'
  import Counter from './lib/Counter.svelte' 
  import Fruits from './components/Fruits.svelte';
  let fruits = ['Apple','Banana','Cherry','Orange','Mango'];
</script>
<Fruits fruits={fruits}/>
<Fruits fruits={fruits} reverse={true}/>
<Fruits fruits={fruits} slice="-2"/>
<Fruits fruits={fruits} slice="0, 3"/>