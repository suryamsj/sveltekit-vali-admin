<svelte:head>
	<title>Lockscreen - Vali Admin</title>
</svelte:head>

<section class="material-half-bg">
	<div class="cover"></div>
</section>
<section class="lockscreen-content">
	<div class="logo">
		<h1>Vali</h1>
	</div>
	<div class="lock-box">
		<img
			class="rounded-circle user-image"
			src="https://randomuser.me/api/portraits/men/1.jpg"
			alt="Men"
		/>
		<h4 class="text-center user-name">John Doe</h4>
		<p class="text-center text-muted">Account Locked</p>
		<form class="unlock-form" action="/">
			<div class="mb-3">
				<label for="text" class="control-label">PASSWORD</label>
				<input class="form-control" type="password" placeholder="Password" />
			</div>
			<div class="mb-3 btn-container d-grid">
				<button class="btn btn-primary btn-block" type="submit"
					><i class="bi bi-unlock me-2 fs-5"></i>UNLOCK
				</button>
			</div>
		</form>
		<p><a href="/login">Not John ? Login Here.</a></p>
	</div>
</section>
