<script lang="ts">
	import { skillList } from './skillList';
	const categories = Object.keys(skillList);
</script>

<h2>Skills</h2>

{#each categories as category}
	<h3>{category}</h3>
	<ul class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-4 gap-2">
		{#each skillList[category] as skill}
			<li class="card variant-soft-primary p-2">{skill.name}</li>
		{/each}
	</ul>
{/each}
