<script lang="ts">
	import { ModeWatcher } from 'mode-watcher';
	import '../app.css';
	import Navbar from '@/navbar.svelte';
	import Footer from '@/footer.svelte';
	let { children } = $props();
</script>

<ModeWatcher />
<Navbar />
<div class="flex min-h-dvh w-full items-center px-10">
	{@render children()}
</div>
<Footer />
