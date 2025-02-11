<script lang="ts">
    let { items } = $props();
</script>

<div class="stats">
{#each items as item}
    <div class="stat">
        <div class="stat-title">{item[0]}</div>
        <div class="stat-value text-primary">{item[1]}</div>
        <div class="stat-desc">{item[2]}</div>
    </div>
{/each}
</div>
