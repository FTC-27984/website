<script lang="ts">
	import './layout.css';
	import Nav from '$lib/components/Nav.svelte';
	import Footer from '$lib/components/Footer.svelte';

	const { children } = $props();
</script>

<div class="flex min-h-screen flex-col bg-black">
	<Nav />
	<main class="flex flex-1 flex-col">
		{@render children()}
	</main>
	<Footer />
</div>
