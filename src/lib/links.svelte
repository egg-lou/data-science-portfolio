<script lang="ts">
	let props = $props();
	let orientation = props.orientation || 'row';
	import { page } from '$app/stores';

	type Link = {
		name: string;
		href: string;
	};

	let pageLinks: Link[] = [
		{ name: 'Home', href: '/' },
		{ name: 'Midterm', href: '/midterm' },
		{ name: 'Final', href: '/final-exam' },
		{ name: 'Contact', href: '/contact' }
	];
</script>

<div class="flex gap-3 {orientation === 'row' ? 'flex-row' : 'flex-col pt-7'}">
	{#each pageLinks as { name, href }}
		<a
			{href}
			class="text-md font-semibold text-gray-800 transition-colors duration-500 hover:text-purple-600 dark:text-gray-200 dark:hover:text-purple-400 {$page
				.url.pathname === href
				? 'border-b-2 border-purple-600'
				: ''}"
		>
			{name}
		</a>
	{/each}
</div>
