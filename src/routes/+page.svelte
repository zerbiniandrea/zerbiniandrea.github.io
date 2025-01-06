<script lang="ts">
	import ContentCard from '../components/ContentCard.svelte';
	import MainCard from '../components/MainCard.svelte';

	const avatarUrl = 'https://avatars.githubusercontent.com/u/43417875?v=4';
</script>

<div class="container mx-auto flex">
	<!-- MainCard stays fixed on the left -->
	<MainCard {avatarUrl} />

	<!-- ContentCard takes the remaining screen space -->
	<div class="flex-grow">
		<ContentCard />
	</div>
</div>
