<script lang="ts">
	import { i18n } from '$lib/i18n';
	import { ParaglideJS } from '@inlang/paraglide-sveltekit';
	import '../app.css';
    import Header from "$lib/Header.svelte";
    import Footer from "$lib/Footer.svelte";
	let { children } = $props();
</script>

<ParaglideJS {i18n}>
    <Header />
	{@render children()}
    <Footer />
</ParaglideJS>
