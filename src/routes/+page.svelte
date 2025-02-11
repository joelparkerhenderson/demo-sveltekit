<script lang="ts">
	import Stat from '$lib/daisyui/Stat.svelte';
	import Stats from '$lib/daisyui/Stats.svelte';
    let stat = { title: 'Alfa', value: 'Bravo'};
	let stats = [
		{ title: 'Charlie', value: 'Delta'},
		{ title: 'Echo', value: 'Foxtrot'}
	];
</script>

<h1>Welcome to SvelteKit</h1>

<hr>

<Stat {stat} />

<hr>

<div class="stats">
	{#each stats as stat}
		<Stat {stat} />
	{/each}
</div>

<hr>

<Stats {stats} />
