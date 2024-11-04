<script lang="ts">
	import logo from '$lib/assets/icon.png';
	import ThemeSwitcher from '$lib/theme-switcher.svelte';
	import * as Sheet from '$lib/components/ui/sheet';
	import { Menu } from 'lucide-svelte';
	import Links from './links.svelte';
</script>

<nav
	class="sticky top-0 flex h-16 w-full items-center justify-between border-b-2 bg-transparent px-6 backdrop-blur"
>
	<div class="flex items-center gap-2">
		<img src={logo} alt="logo" class="h-5 w-5" />
		<h1 class="text-md font-semibold">Rafael Miguel | BSIT 3 - 5</h1>
	</div>
	<div class="flex items-center gap-3">
		<ThemeSwitcher />
		<div class="hidden items-center gap-3 lg:flex">
			<Links orientation="row" />
		</div>
		<div class="flex lg:hidden">
			<Sheet.Root>
				<Sheet.Trigger><Menu class="h-5 w-5" /></Sheet.Trigger>
				<Sheet.Content>
					<Sheet.Header>
						<Sheet.Title class="flex items-center pt-5">
							<img src={logo} alt="logo" class="h-5 w-5" />
							<h1 class="text-md font-semibold">Rafael Miguel | BSIT 3 - 5</h1>
						</Sheet.Title>
					</Sheet.Header>
					<Sheet.Description>
						<Links orientation="column" />
					</Sheet.Description>
				</Sheet.Content>
			</Sheet.Root>
		</div>
	</div>
</nav>
