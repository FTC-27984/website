<script lang="ts">
	const socials = [
		{ href: 'https://github.com/ftc-27984', label: 'GitHub' },
		{ href: 'https://ftcscout.org/teams/27984', label: 'FTCScout' }
	];
</script>

<footer class="flex flex-col gap-4 px-6 py-8 text-sm text-white/60 sm:flex-row sm:items-center sm:justify-between sm:px-10">
	<p>&copy; {new Date().getFullYear()} FTC 27984 — Viewmount Elves</p>
	<div class="flex gap-5">
		{#each socials as social}
			<a
				href={social.href}
				target="_blank"
				rel="noopener noreferrer"
				class="transition-colors hover:text-white">{social.label}</a
			>
		{/each}
	</div>
</footer>
