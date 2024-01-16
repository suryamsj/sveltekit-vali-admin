<script>
	import { page } from '$app/stores';

	export let title = '';
	export let desc = '';
	export let iconTitle = '';

	const url = $page.url.pathname;
</script>

<div class="app-title">
	<div>
		<h1><i class={iconTitle}></i> {title}</h1>
		<p>{desc}</p>
	</div>
	<ul class="app-breadcrumb breadcrumb">
		<li class="breadcrumb-item"><i class="bi bi-house-door fs-6"></i></li>
		<li class="breadcrumb-item"><a href={url}>{title}</a></li>
	</ul>
</div>
