<script>
	import AppTitle from '$lib/components/AppTitle.svelte';
</script>

<svelte:head>
	<title>Widgets - Vali Admin</title>
</svelte:head>

<AppTitle title="Widgets" desc="Widgets to interactively display data" iconTitle="bi bi-archive" />

<div class="row">
	<div class="col-md-3">
		<div class="widget-small primary">
			<i class="icon bi bi-people fs-1"></i>
			<div class="info">
				<h4>Users</h4>
				<p><b>5</b></p>
			</div>
		</div>
	</div>
	<div class="col-md-3">
		<div class="widget-small info">
			<i class="icon bi bi-heart fs-1"></i>
			<div class="info">
				<h4>Likes</h4>
				<p><b>25</b></p>
			</div>
		</div>
	</div>
	<div class="col-md-3">
		<div class="widget-small warning">
			<i class="icon bi bi-folder2 fs-1"></i>
			<div class="info">
				<h4>Uploades</h4>
				<p><b>10</b></p>
			</div>
		</div>
	</div>
	<div class="col-md-3">
		<div class="widget-small danger">
			<i class="icon bi bi-star fs-1"></i>
			<div class="info">
				<h4>Stars</h4>
				<p><b>500</b></p>
			</div>
		</div>
	</div>
</div>
<div class="row">
	<div class="col-md-3">
		<div class="widget-small primary coloured-icon">
			<i class="icon bi bi-people fs-1"></i>
			<div class="info">
				<h4>Users</h4>
				<p><b>5</b></p>
			</div>
		</div>
	</div>
	<div class="col-md-3">
		<div class="widget-small info coloured-icon">
			<i class="icon bi bi-heart fs-1"></i>
			<div class="info">
				<h4>Likes</h4>
				<p><b>25</b></p>
			</div>
		</div>
	</div>
	<div class="col-md-3">
		<div class="widget-small warning coloured-icon">
			<i class="icon bi bi-folder2 fs-1"></i>
			<div class="info">
				<h4>Uploades</h4>
				<p><b>10</b></p>
			</div>
		</div>
	</div>
	<div class="col-md-3">
		<div class="widget-small danger coloured-icon">
			<i class="icon bi bi-star fs-1"></i>
			<div class="info">
				<h4>Stars</h4>
				<p><b>500</b></p>
			</div>
		</div>
	</div>
</div>
<div class="row">
	<div class="col-md-6">
		<div class="tile">
			<h3 class="tile-title">Chat</h3>
			<div class="messanger">
				<div class="messages">
					<div class="message">
						<img src="https://randomuser.me/api/portraits/men/4.jpg" alt="Man" />
						<p class="info">Hello there!<br />Good Morning</p>
					</div>
					<div class="message me">
						<img src="https://randomuser.me/api/portraits/men/1.jpg" alt="Man" />
						<p class="info">Hi<br />Good Morning</p>
					</div>
					<div class="message">
						<img src="https://randomuser.me/api/portraits/men/4.jpg" alt="Man" />
						<p class="info">How are you?</p>
					</div>
					<div class="message me">
						<img src="https://randomuser.me/api/portraits/men/1.jpg" alt="Man" />
						<p class="info">I'm Fine.</p>
					</div>
				</div>
				<div class="sender">
					<input type="text" placeholder="Send Message" />
					<button class="btn btn-primary" type="button" aria-label="send"><i class="bi bi-send fs-5"></i></button>
				</div>
			</div>
		</div>
	</div>
</div>
