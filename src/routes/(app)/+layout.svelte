<script>
	import Navbar from '$lib/components/Navbar.svelte';
	import Sidebar from '$lib/components/Sidebar.svelte';
	import Transition from '$lib/components/Transition.svelte';

	export let data;
</script>

<!-- Navbar -->
<Navbar />

<!-- Sidebar -->
<Sidebar />
<main class="app-content">
	<Transition key={data.pathname} duration={400}>
		<slot />
	</Transition>
</main>
