<script lang="ts">
	import { Sun, Moon } from 'lucide-svelte';
	import { toggleMode } from 'mode-watcher';
	import { Button } from '$lib/components/ui/button/index';
</script>

<Button onclick={toggleMode} variant="ghost" size="icon">
	<Sun class="hidden h-[1.2rem] w-[1.2rem] dark:block" />
	<Moon class="block h-[1.2rem] w-[1.2rem] dark:hidden" />
	<span class="sr-only">Toggle Theme</span>
</Button>
