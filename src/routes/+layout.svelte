<script>
	import { browser } from '$app/environment';
	import '../app.scss';

	let { children } = $props();

	$effect(() => {
		(async () => {
			if (!browser) return;

			import('bootstrap');
		})();
	});
</script>

{@render children()}
