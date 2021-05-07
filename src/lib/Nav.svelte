<script>
	import { page } from '$app/stores';
</script>


<nav>
	<a class:selected={$page.path === '/'} sveltekit:prefetch href="/">Home</a>
	<a class:selected={$page.path === '/about'} sveltekit:prefetch href="/about">About</a>
</nav>


<style>
	a {
		margin: 0.25em;
		text-decoration: none;
	}
</style>
