<script>
	import AppTitle from '$lib/components/AppTitle.svelte';
</script>

<svelte:head>
	<title>Cards - Vali Admin</title>
</svelte:head>

<AppTitle title="Cards" desc="Material design inspired cards" iconTitle="bi bi-laptop" />

<!-- svelte-ignore a11y-invalid-attribute -->
<div class="row">
	<div class="col-md-6">
		<div class="tile">
			<h3 class="tile-title">Card Title</h3>
			<div class="tile-body">
				Hey there, I am a very simple card. I am good at containing small bits of information. I am
				quite convenient because I require little markup to use effectively.
			</div>
			<div class="tile-footer"><a class="btn btn-primary" href="#">Link</a></div>
		</div>
	</div>
	<div class="col-md-6">
		<div class="tile">
			<div class="tile-title-w-btn">
				<h3 class="title">All Items</h3>
				<p>
					<a class="btn btn-primary icon-btn" href=""
						><i class="bi bi-plus-square me-2"></i>Add Item
					</a>
				</p>
			</div>
			<div class="tile-body">
				<b>Card with action button </b><br />
				Hey there, I am a very simple card. I am good at containing small bits of information. I am quite
				convenient because I require little markup to use effectively.
			</div>
		</div>
	</div>
	<div class="clearfix"></div>
	<div class="col-md-6">
		<div class="tile">
			<div class="tile-title-w-btn">
				<h3 class="title">All Items</h3>
				<div class="btn-group">
					<a class="btn btn-primary" href="#"><i class="bi bi-plus-square fs-5"></i></a><a
						class="btn btn-primary"
						href="#"><i class="bi bi-pencil-square fs-5"></i></a
					><a class="btn btn-primary" href="#"><i class="bi bi-trash fs-5"></i></a>
				</div>
			</div>
			<div class="tile-body">
				<b>Card with button group </b><br />
				Hey there, I am a very simple card. I am good at containing small bits of information. I am quite
				convenient because I require little markup to use effectively.
			</div>
		</div>
	</div>
	<div class="col-md-6">
		<div class="tile">
			<div class="overlay">
				<div class="m-loader mr-4">
					<svg class="m-circular" viewBox="25 25 50 50">
						<circle
							class="path"
							cx="50"
							cy="50"
							r="20"
							fill="none"
							stroke-width="4"
							stroke-miterlimit="10"
						/>
					</svg>
				</div>
				<h3 class="l-text">Loading</h3>
			</div>
			<div class="tile-title-w-btn">
				<h3 class="title">All Items</h3>
				<p>
					<a class="btn btn-primary icon-btn" href="/"
						><i class="bi bi-plus-square"></i>Add Item
					</a>
				</p>
			</div>
			<div class="tile-body">
				<b>Card with action button </b><br />
				Hey there, I am a very simple card. I am good at containing small bits of information. I am quite
				convenient because I require little markup to use effectively.
			</div>
		</div>
	</div>
</div>
