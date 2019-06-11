<script>
	export let name;

	let rando;

	$: result = Math.round(rando) ? 'winner' : 'loser'

	function setRando() {
		rando = Math.random()
	}

</script>

<style>
	h1 {
		color: purple;
	}
</style>

<h1>Welcome to {name}!</h1>
<p>The random number is { rando }</p>
<input bind:value={ rando }>
<p>{ result }</p>
<button on:click={setRando}>Randomize</button>