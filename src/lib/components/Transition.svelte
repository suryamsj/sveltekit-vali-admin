<script>
	import { cubicInOut } from 'svelte/easing';
	import { fade } from 'svelte/transition';

	/** @type {{key?: string, duration?: number, children?: import('svelte').Snippet}} */
	let { key = '', duration = 300, children } = $props();
</script>

{#key key}
	<div
		in:fade={{ easing: cubicInOut, duration, delay: duration }}
		out:fade={{ easing: cubicInOut, duration }}
	>
		{@render children?.()}
	</div>
{/key}
