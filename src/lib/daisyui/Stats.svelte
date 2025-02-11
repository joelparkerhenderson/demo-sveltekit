<script lang="ts">
	import Stat from '$lib/daisyui/Stat.svelte';
    let { stats } = $props();
</script>

<div class="stats">
{#each stats as stat}
    <Stat {stat} />
{/each}
</div>
