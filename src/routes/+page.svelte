<script>
	let firstName = 'Rashmika';
	let lastName = 'Lakshan';

	$: name = `${firstName} ${lastName}`;
	$: {
		console.log(firstName);
		console.log(lastName);
		console.log(name);
	}
	//if value change run the all code block
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

	input {
		margin-bottom: 1rem;
		width: 50%;
		padding: 0.5rem;
		font-size: 1rem;
		border: 1px solid #6b6464;
		border-radius: 0.25rem;
		box-sizing: border-box;
	}
</style>
