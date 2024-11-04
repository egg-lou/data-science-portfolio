<script lang="ts">
	import { ModeWatcher } from 'mode-watcher';
	import '../app.css';
	import Navbar from '@/navbar.svelte';
	import Footer from '@/footer.svelte';
	let { children } = $props();
</script>

<ModeWatcher />
<div class="min-h-screen">
	<div class="relative flex min-h-dvh flex-col">
		<Navbar />
		<main class="container mx-auto max-w-7xl flex-grow px-6 pb-5 pt-5">
			{@render children()}
		</main>
		<Footer />
	</div>
</div>
