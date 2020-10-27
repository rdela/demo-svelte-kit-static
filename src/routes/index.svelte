<script>
	import Counter from '$components/Counter.svelte';
</script>

<header>
	<h1>Hello 🌍!</h1>
</header>

<div class="touch-action-manipulation">
	<Counter/>
</div>

<article>
	<p>Visit <a href="https://svelte.dev">svelte.dev</a> to learn how to build Svelte apps or learn more <a href="/about">about this site</a>.</p>
</article>


<style>
	.touch-action-manipulation {
		touch-action: manipulation;
	}

	header {
		padding: 1rem 2rem;
	}
</style>
