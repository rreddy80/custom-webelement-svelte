<script>
	let count = 0;

	function handleClick() {
		count += 1;
	}

	function resetCounter() {
		count = 0;
	}
</script>

<button on:click={handleClick}>
	Clicked {count} {count === 1 ? 'time' : 'times'}
</button>

<button on:click={resetCounter}>Reset Counter</button>

<svelte:options tag="count-btn" />
