<script>
	import { browser } from '$app/environment';

	$effect(() => {
		(async () => {
			if (!browser) return;

			let flipButtons = document.querySelectorAll('.login-content [data-toggle="flip"]');
			let loginBox = document.querySelector('.login-box');

			flipButtons.forEach((flipButton) => {
				// @ts-ignore
				flipButton.addEventListener('click', function (e) {
					e.preventDefault();
					loginBox?.classList.toggle('flipped');
					return false;
				});
			});
		})();
	});
</script>

<svelte:head>
	<title>Login - Vali Admin</title>
</svelte:head>

<section class="material-half-bg">
	<div class="cover"></div>
</section>
<section class="login-content">
	<div class="logo">
		<h1>Vali</h1>
	</div>
	<div class="login-box">
		<form class="login-form" action="/">
			<h3 class="login-head"><i class="bi bi-person me-2"></i>SIGN IN</h3>
			<div class="mb-3">
				<label for="text" class="form-label">USERNAME</label>
				<input class="form-control" type="text" placeholder="Email" />
			</div>
			<div class="mb-3">
				<label for="text" class="form-label">PASSWORD</label>
				<input class="form-control" type="password" placeholder="Password" />
			</div>
			<div class="mb-3">
				<div class="utility">
					<div class="form-check">
						<label class="form-check-label">
							<input class="form-check-input" type="checkbox" /><span class="label-text"
								>Stay Signed in</span
							>
						</label>
					</div>
					<p class="semibold-text mb-2"><button style="background: none; border: none; text-decoration: underline; color: #00695c" data-toggle="flip">Forgot Password ?</button></p>
				</div>
			</div>
			<div class="mb-3 btn-container d-grid">
				<button class="btn btn-primary btn-block"
					><i class="bi bi-box-arrow-in-right me-2 fs-5"></i>SIGN IN</button
				>
			</div>
		</form>
		<form class="forget-form" action="/">
			<h3 class="login-head"><i class="bi bi-person-lock me-2"></i>Forgot Password ?</h3>
			<div class="mb-3">
				<label for="text" class="form-label">EMAIL</label>
				<input class="form-control" type="text" placeholder="Email" />
			</div>
			<div class="mb-3 btn-container d-grid">
				<button class="btn btn-primary btn-block"
					><i class="bi bi-unlock me-2 fs-5"></i>RESET</button
				>
			</div>
			<div class="mb-3 mt-3">
				<p class="semibold-text mb-0">
					<button style="background: none; border: none; text-decoration: underline; color: #00695c" data-toggle="flip"><i class="bi bi-chevron-left me-1"></i> Back to Login</button>
				</p>
			</div>
		</form>
	</div>
</section>
