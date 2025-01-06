<script>
	const languages = [
		{
			name: 'JavaScript',
			description: 'A versatile language primarily used for web development.'
		},
		{
			name: 'Python',
			description: 'A powerful language for data science, AI, and backend development.'
		},
		{
			name: 'Java',
			description: 'Widely used for enterprise solutions and Android app development.'
		},
		{
			name: 'C++',
			description: 'A high-performance language for system programming and game development.'
		},
		{
			name: 'Go',
			description: 'A language for building scalable and efficient backend systems.'
		}
	];
</script>

<div class="grid" style="gap: 1rem; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); margin: 1rem;">
	{#each languages as language}
		<card class="card-hover variant-outline-tertiary bg-surface-500 rounded-2xl shadow-xl overflow-hidden p-4 w-full text-token flex flex-col">
			<header class="card p-4 flex rounded-t-2xl shadow-xl justify-center items-center">
				<h3 class="h3">{language.name}</h3>
			</header>
			<div class="p-4 space-y-4 flex-grow">
				<p class="opacity-75">{language.description}</p>
			</div>
		</card>
	{/each}
</div>
