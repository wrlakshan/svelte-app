<script>
	let name = 'Rashmika';
	let num = 1;
	const handleClick = () => {
		num = num + 1;
	};
</script>

<main>
	<h1>Welcome to {name} {num}</h1>
	<button on:click={handleClick}>update the color</button>
	<input type="text" bind:value={name} /> //two way data binding
</main>

<style>
	main {
		text-align: center;
	}

	h1 {
		font-size: 2rem;
		color: #178882;
		text-align: center;
		margin-top: 4em;
	}
</style>
