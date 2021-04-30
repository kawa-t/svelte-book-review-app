<form>
<form on:submit|preventDefault={handleSubmit}></form>
  <SearchBar bind:value={q} />
</form>

<div class="text-center mt-4">
  { q }
</div>

<script>
 import SearchBar from "../components/SearchBar.svelte";

 let q = 'JavaScript'

const handleSubmit = () => {
  console.log('handleSubmit')
  console.log(q)
}
</script>
