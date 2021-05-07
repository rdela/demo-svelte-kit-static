<script>
	import Nav from '$lib/Nav.svelte';
</script>


<main>
	<Nav/>
	<slot></slot>
</main>


<style>
	main {
		display: block;
		margin: 0 auto;
		padding: 1rem;
		text-align: center;
	}
</style>
