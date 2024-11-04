<script lang="ts">
	import { HardHat } from 'lucide-svelte';
	import { Button } from '$lib/components/ui/button/index';
</script>

<div class="flex flex-col items-center rounded-lg border-2 p-8 shadow-xl">
	<div class="mb-6 flex justify-center">
		<div class="animate-bounce rounded-full bg-yellow-400 p-4">
			<HardHat className="h-12 w-12 text-gray-800" />
		</div>
	</div>
	<h1 class="mb-4 text-4xl font-bold">Under Construction</h1>
	<p class="mb-8 text-lg text-muted-foreground">
		We're working hard to bring you something amazing. Please check back soon!
	</p>
	<div class="flex justify-center space-x-4">
		<Button variant="default">
			<a href="/">Return Home</a>
		</Button>
	</div>
</div>
