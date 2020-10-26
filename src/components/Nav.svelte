<script>
	export let segment;
</script>


<nav>
	<a class="{segment === undefined ? 'selected' : undefined}" href="/">Home</a>
	<a class="{segment === 'about' ? 'selected' : undefined}" href="/about">About</a>
</nav>


<style>
	a {
		margin: 0.25em;
		text-decoration: none;
	}
</style>
