<script>
	import { count } from './stores.js';
	import Decrementer from './Decrementer.svelte';
	import Incrementer from './Incrementer.svelte';
	import Resetter from './Resetter.svelte';

	export let tally = 0;

	const decrement = () => {
		tally -= 1;
	};

	const increment = () => {
		tally += 1;
	};

	const reset = () => {
		tally = 0;
	};
</script>

<section>
	<!-- Any name beginning with $ is assumed to refer to a store value.
	 It's effectively a reserved character — Svelte will prevent you from
	 declaring your own variables with a $ prefix. -->
	<h2>The count is {$count}</h2>
	<!-- You're not limited to using $count inside the markup, either —
	 you can use it anywhere in the <script> as well, such as in event
	 handlers or reactive declarations.
	Auto-subscription only works with store variables that are declared
	 (or imported) at the top-level scope of a component. -->

	<Incrementer/>
	<Decrementer/>
	<Resetter/>
</section>

<section>
	<h2>The tally is {tally}</h2>

	<button on:click={increment}>
		+
	</button>

	<button on:click={decrement}>
		-
	</button>

	<button on:click={reset}>
		reset
	</button>
</section>

<article>
	<p>
		This example (derived from the
		 <a href="https://svelte.dev/tutorial/writable-stores">Writable stores</a>
		 and
		 <a href="https://svelte.dev/tutorial/auto-subscriptions">Auto-subscriptions</a>
		 sections of the
		 <a href="https://svelte.dev/tutorial/basics">Svelte Tutorial</a>)
		 illustrates two different approaches to building a
		 counter component, one using a
		 <a href="https://svelte.dev/docs#svelte_store">writable store</a>
		 to hold the “count” value, and the other using a
		 <a href="https://svelte.dev/tutorial/adding-data">variable declared
		 in the component</a> to hold the “tally” value.
	</p>
	<p>
		If we set a value on both counters and then navigate to the
		 <a href="/about">About page</a> and back, tally will be reset to 0
		 but count will retain its value. Reloading the page will clear both
		 values.
	</p>
	<p>
		To better understand the difference, have a look at the
		 <a href="https://github.com/rdela/demo-svelte-kit-static/blob/trunk/src/components/Counter.svelte">
		 source code on GitHub</a> and then try
		 <a href="https://svelte.dev/tutorial/basics">the tutorial</a>
		 and/or read through the docs linked above.
	</p>
</article>

<style>
	h2 { margin-top: 0; }
</style>
