<script>
	import { TabGroup, Tab } from '@skeletonlabs/skeleton';
	import ProgrammingSkills from './ProgrammingSkills.svelte';

	let tabsBasic = 0;

	const desc = {
		contacts: 'You can reach me through email or social media. My contact information is listed here.',
		projects: 'A collection of projects I have worked on, including GitHub repositories and demos.',
		about: 'Learn more about me, including my background, skills, and interests.'
	};
</script>

<div
	class="card shadow-2xl variant-ghost overflow-hidden p-4 w-full h-[calc(100vh-2rem)] text-token flex flex-col"
	style="margin: 1rem;"
>
	<header class="rounded-2xl p-4 flex justify-center items-center space-x-4">
		<img class="card-hover rounded-2xl shadow-xl" src="/banner2.png" alt="banner" />
	</header>

	<TabGroup class="h-full" justify="justify-center">
		<!-- Tabs -->
		<div class="flex space-x-4">
			<Tab bind:group={tabsBasic} name="contacts" value={0}>Programming Skills</Tab>
			<Tab bind:group={tabsBasic} name="projects" value={1}>About Me</Tab>
			<Tab bind:group={tabsBasic} name="about" value={2}>Hobbies</Tab>
			<Tab bind:group={tabsBasic} name="about" value={3}>Contacts</Tab>
			<Tab bind:group={tabsBasic} name="about" value={4}>CV</Tab>
		</div>

		<!-- Panel -->
		<svelte:fragment slot="panel">
			<div class="h-full p-4">
				{#if tabsBasic === 0}
					<ProgrammingSkills />
				{:else if tabsBasic === 1}
					<p>{desc.projects}</p>
				{:else if tabsBasic === 2}
					<p>{desc.about}</p>
				{/if}
			</div>
		</svelte:fragment>
	</TabGroup>
</div>
