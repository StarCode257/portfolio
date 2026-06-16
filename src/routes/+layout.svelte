<script lang="ts">
	import './layout.css';
	import favicon from '$lib/assets/favicon.svg';

	let { children } = $props();
</script>

<svelte:head><link rel="icon" href={favicon} /></svelte:head>

<header class="flex justify-between p-4">
	<span>Diamant</span>
	<nav class="flex gap-8">
		<a href="#">About</a>
		<a href="#">Services</a>
		<a href="#">Contact</a>
	</nav>
	<span> +257 62 277 058 </span>
</header>

{@render children()}

<footer class="flex justify-center">@copy starcode257</footer>
