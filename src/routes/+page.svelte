<script>
	let peoples = [
		{ id: 1, name: 'John', age: 20, email: 'john@example.com' },
		{ id: 2, name: 'Mary', age: 20, email: 'Mary@example.com' },
		{ id: 3, name: 'kids', age: 20, email: 'kids@example.com' }
	];
</script>

<main>
	{#each peoples as person (person.id)}
		<div>
			<h1>{person.name}</h1>
			<p>{person.age}</p>
			<p>{person.email}</p>
		</div>
	{:else}
		<div>
			<h1>No people found</h1>
		</div>
	{/each}
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
		margin-top: 2em;
	}

	p {
		font-size: 1rem;
		color: #569e9a;
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
