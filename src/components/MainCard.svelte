<script>
	import { Avatar } from '@skeletonlabs/skeleton';

	export let avatarUrl = '';
</script>

<div
	class="card shadow-xl variant-ghost overflow-hidden max-w-[400px] w-full h-[calc(100vh-2rem)] text-token flex flex-col"
	style="margin: 1rem;"
>
	<header class="card variant-soft p-4 flex justify-center items-center space-x-4">
		<Avatar src={avatarUrl} width="w-40" rounded="rounded-full" border="border-2">
			<Avatar initials="AZ" background="bg-primary-500" />
		</Avatar>
	</header>
	<hr class="!border-t-2" />
	<div class="p-4 space-y-4 flex-grow">
		<h6 class="h6">Software Developer</h6>
		<h3 class="h3">Zerbini Andrea</h3>
		<article>
			<p class="opacity-75">
				Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed euismod, nisl eget ultricies aliquam, nisi nisl
				aliquet nisi, in vehicula nisl
			</p>
		</article>
	</div>
	<hr class="!border-t-2" />
	<footer class="p-2 flex justify-center items-center space-x-4">
		<div class="flex justify-center space-x-2">
			<a href="#" class="chip variant-soft hover:variant-filled"
				><i class="fa-solid fa-heart"></i> <span>Github</span></a
			>
			<a href="#" class="chip variant-soft hover:variant-filled"
				><i class="fa-solid fa-paperclip"></i> <span>LinkedIn</span></a
			>
			<a href="#" class="chip variant-soft hover:variant-filled"><i class="fa-solid fa-share"></i> <span>Boh</span></a>
		</div>
	</footer>
</div>
