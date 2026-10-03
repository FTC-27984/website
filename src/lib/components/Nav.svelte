<script lang="ts">
	const links = [
		{ href: '/team', label: 'Team' },
		{ href: '/season', label: 'Season' },
		{ href: '/sponsors', label: 'Sponsors' }
	];
</script>

<nav class="flex items-center justify-between px-6 py-4 text-white sm:px-10">
	<a href="/" class="text-sm font-semibold tracking-wide">27984</a>
	<div class="flex gap-6 text-sm text-white/70">
		{#each links as link}
			<a href={link.href} class="transition-colors hover:text-white">{link.label}</a>
		{/each}
	</div>
</nav>
