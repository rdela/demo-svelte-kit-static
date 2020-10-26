<script>
	export let count = 0;

	const decrement = () => {
		count -= 1;
	};

	const increment = () => {
		count += 1;
	};
</script>


<p>
	Tally: {count}
</p>

<button on:click={decrement}>
	-
</button>

<button on:click={increment}>
	+
</button>


<style>
	button {
		font-family: inherit;
		font-size: inherit;
		margin: 0 0.5em 1em;
		padding: 1rem;
		color: #ff3e00;
		background-color: rgba(255, 62, 0, 0.3);
		border-radius: 2em;
		border: 2px solid rgba(255, 62, 0, 0);
		outline: none;
		width: 6rem;
		font-variant-numeric: tabular-nums;
	}

	button:focus {
		border: 2px solid #ff3e00;
	}

	button:active {
		background-color: rgba(255, 62, 0, 0.2);
	}
</style>
