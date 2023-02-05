<script lang="ts">
	const socials = [
		{
			name: 'GitHub',
			href: 'https://github.com/keithrpotempa',
			icon: 'github'
		},
		{
			name: 'LinkedIn',
			href: 'https://www.linkedin.com/in/keithrpotempa/'
		},
		{
			name: 'Twitter',
			href: 'https://twitter.com/keithrpotempa',
			icon: 'twitter'
		},
		{
			name: 'Resume',
			href: 'https://res.cloudinary.com/krp/image/upload/v1614724673/keithpotempa.com/Potempa_Dev_Resume_v9.pdf'
		}
	];
</script>

{#each socials as social}
	<a class="btn btn-sm variant-ghost-surface" href={social.href} target="_blank" rel="noreferrer"
		>{social.name}</a
	>
{/each}
