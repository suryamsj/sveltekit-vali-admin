<script>
	import { cubicInOut } from 'svelte/easing';
	import { fade } from 'svelte/transition';

	export let key = '';
	export let duration = 300;
</script>

{#key key}
	<div
		in:fade={{ easing: cubicInOut, duration, delay: duration }}
		out:fade={{ easing: cubicInOut, duration }}
	>
		<slot />
	</div>
{/key}
