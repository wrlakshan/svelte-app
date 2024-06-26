<script>
	let firstName = 'Rashmika';
	let lastName = 'Lakshan';
	$: name = firstName + ' ' + lastName;
</script>

<main>
	<h1>{name}</h1>
	<input type="text" bind:value={firstName} />
	<input type="text" bind:value={lastName} />
</main>

<style>
	main {
		text-align: center;
		padding: 4rem;
	}

	h1 {
		font-size: 2rem;
		color: #178882;
		text-align: center;
		margin-top: 4em;
	}
</style>
