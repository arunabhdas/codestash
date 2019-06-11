<script>
	export let name;

	let rando;

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
<button on:click={setRando}>Randomize</button>