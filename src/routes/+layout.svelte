<script lang="ts">
	import './layout.css';
	import favicon from '$lib/assets/favicon.svg';
	import { page } from '$app/state';
	import { resolve } from '$app/paths';
	import { cn } from '$lib/utils';
	import * as Drawer from '$lib/components/ui/drawer/index.js';
	import Button from '$lib/components/ui/button/button.svelte';

	let open = $state(false);
	let { children } = $props();
	let pathname = $derived(page.url.pathname);
	function isActive(current: string) {
		console.log(pathname);
		return pathname == current ? 'border-x-primary' : 'border-transparent';
	}
</script>

<svelte:head><link rel="icon" href={favicon} /></svelte:head>

<header class="flex flex-wrap items-center justify-between p-4 md:px-16">
	<div class="flex items-center gap-2">
		<div class="md:hidden">
			<Drawer.Root direction="left" bind:open>
				<Drawer.Trigger>
					<Button variant="outline"><i class="fa fa-bars"></i></Button>
				</Drawer.Trigger>
				<Drawer.Content>
					<Drawer.Header>
						<div class="flex justify-end">
							<Button variant="ghost" onclick={() => (open = false)}
								><i class="fa fa-times"></i></Button
							>
						</div>
					</Drawer.Header>
					<nav class="flex flex-col gap-8 p-8">
						<a
							href={resolve('/')}
							onclick={() => (open = false)}
							class={cn(isActive('/'), 'rounded-3xl border-x-2 px-2 hover:border-x-primary')}
							>About</a
						>
						<a
							href={resolve('/services')}
							onclick={() => (open = false)}
							class={cn(
								isActive('/services'),
								'rounded-3xl border-x-2  px-2 hover:border-x-primary'
							)}>Services</a
						>
						<a
							href={resolve('/contact')}
							onclick={() => (open = false)}
							class={cn(isActive('/contact'), 'rounded-3xl border-x-2 px-2 hover:border-x-primary')}
							>Contact</a
						>
					</nav>
				</Drawer.Content>
			</Drawer.Root>
		</div>
		<span class="marck-script-regular text-6xl">Diamant</span>
	</div>
	<nav class="hidden gap-8 md:flex">
		<a
			href={resolve('/')}
			class={cn(isActive('/'), 'rounded-3xl border-x-2 px-2 hover:border-x-primary')}>About</a
		>
		<a
			href={resolve('/services')}
			class={cn(isActive('/services'), 'rounded-3xl border-x-2  px-2 hover:border-x-primary')}
			>Services</a
		>
		<a
			href={resolve('/contact')}
			class={cn(isActive('/contact'), 'rounded-3xl border-x-2 px-2 hover:border-x-primary')}
			>Contact</a
		>
	</nav>
	<span> +257 62 277 058 <i class="fab fa-whatsapp"></i></span>
</header>

{@render children()}

<footer class="flex justify-center">@copy starcode257</footer>
