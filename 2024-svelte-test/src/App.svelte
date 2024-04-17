<script>
  import svelteLogo from './assets/svelte.svg'
  import viteLogo from '/vite.svg'
  import Counter from './lib/Counter.svelte' 
  import { storeName } from './store.js';
  import Fruits from './components/Fruits.svelte';
  import Parent from './components/Parent.svelte';
  import Child from './components/Child.svelte';
  let fruits = ['Apple','Banana','Cherry','Orange','Mango'];
  let word = 'world';
  $storeName = word
</script>
<Fruits fruits={fruits}/>
<Fruits fruits={fruits} reverse={true}/>
<Fruits fruits={fruits} slice="-2"/>
<Fruits fruits={fruits} slice="0, 3"/>
<Parent/>