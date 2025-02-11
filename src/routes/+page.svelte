<script lang="ts">
	import Stat from '$lib/daisyui/Stat.svelte';
	import Stats from '$lib/daisyui/Stats.svelte';
	let items = [
		['Title A', 'Value B', 'Description C'],
		['Title D', 'Value E', 'Description F'],
		['Title G', 'Value H', 'Description I']
	];
</script>

<h1>Welcome to SvelteKit</h1>

<Stat 
	title="My Title" 
	value="My Value" 
	description="My Description" 
/>

<Stats {items} />
