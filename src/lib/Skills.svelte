<script lang="ts">
	import { skillList } from './skillList';
	const categories = Object.keys(skillList);
</script>

{#each categories as category}
	<h2>{category}</h2>
	<div class="logo-cloud grid-cols-1 lg:grid-cols-4 gap-1">
		{#each skillList[category] as skill}
			<div class="logo-item">{skill.name}</div>
		{/each}
	</div>
{/each}
