<script lang="ts">
	import type { AvailableLanguageTag } from '$lib/paraglide/runtime';
	import { i18n } from '$lib/i18n';
	import { page } from '$app/stores';
	import { goto } from '$app/navigation';
	import * as m from '$lib/paraglide/messages.js';

	function switchToLanguage(newLanguage: AvailableLanguageTag) {
		const canonicalPath = i18n.route($page.url.pathname);
		const localisedPath = i18n.resolveRoute(canonicalPath, newLanguage);
		goto(localisedPath);
	}
</script>

<h1>{m.hello_world({ name: 'SvelteKit User' })}</h1>
<div>
	<button onclick={() => switchToLanguage('ar')}>ar</button>
	<button onclick={() => switchToLanguage('cy')}>cy</button>
	<button onclick={() => switchToLanguage('de')}>de</button>
	<button onclick={() => switchToLanguage('en')}>en</button>
	<button onclick={() => switchToLanguage('es')}>es</button>
	<button onclick={() => switchToLanguage('eu')}>eu</button>
	<button onclick={() => switchToLanguage('fr')}>fr</button>
	<button onclick={() => switchToLanguage('hi')}>hi</button>
	<button onclick={() => switchToLanguage('ja')}>ja</button>
	<button onclick={() => switchToLanguage('sv')}>sv</button>
	<button onclick={() => switchToLanguage('ru')}>ru</button>
	<button onclick={() => switchToLanguage('zh')}>zh</button>
</div>
