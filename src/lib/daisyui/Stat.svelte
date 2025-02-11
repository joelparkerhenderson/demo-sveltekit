<script>
	let { stat } = $props();
</script>

<div class="stat">
    {#if stat.title != null}<div class="stat-title">{stat.title}</div>{/if}
    {#if stat.value != null}<div class="stat-value">{stat.value}</div>{/if}
    {#if stat.desc != null}<div class="stat-desc">{stat.desc}</div>{/if}
</div>
