<script>
	import { onMount } from 'svelte';
	import { browser } from '$app/environment';
	import '../app.scss';

	onMount(async () => {
		if (!browser) return;

		await import('bootstrap');
	});
</script>

<slot />
