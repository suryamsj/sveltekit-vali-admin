<script>
	import AppTitle from '$lib/components/AppTitle.svelte';
</script>

<svelte:head>
	<title>Form Samples - Vali Admin</title>
</svelte:head>

<AppTitle title="Form Samples" desc="Sample forms" iconTitle="bi bi-ui-checks" />

<div class="row">
	<div class="col-md-6">
		<div class="tile">
			<h3 class="tile-title">Vertical Form</h3>
			<div class="tile-body">
				<form>
					<div class="mb-3">
						<label for="text" class="form-label">Name</label>
						<input class="form-control" type="text" placeholder="Enter full name" />
					</div>
					<div class="mb-3">
						<label for="text" class="form-label">Email</label>
						<input class="form-control" type="email" placeholder="Enter email address" />
					</div>
					<div class="mb-3">
						<label for="text" class="form-label">Address</label>
						<textarea class="form-control" rows="4" placeholder="Enter your address"></textarea>
					</div>
					<div class="mb-3">
						<label for="text" class="form-label">Gender</label>
						<div class="form-check">
							<label class="form-check-label">
								<input class="form-check-input" type="radio" name="gender" />Male
							</label>
						</div>
						<div class="form-check">
							<label class="form-check-label">
								<input class="form-check-input" type="radio" name="gender" />Female
							</label>
						</div>
					</div>
					<div class="mb-3">
						<label for="text" class="form-label">Identity Proof</label>
						<input class="form-control" type="file" />
					</div>
					<div class="mb-3">
						<div class="form-check">
							<label class="form-check-label">
								<input class="form-check-input" type="checkbox" />I accept the terms and conditions
							</label>
						</div>
					</div>
				</form>
			</div>
			<div class="tile-footer">
				<button class="btn btn-primary" type="button"
					><i class="bi bi-check-circle-fill me-2"></i>Register</button
				>&nbsp;&nbsp;&nbsp;<a class="btn btn-secondary" href="/"
					><i class="bi bi-x-circle-fill me-2"></i>Cancel</a
				>
			</div>
		</div>
	</div>
	<div class="col-md-6">
		<div class="tile">
			<h3 class="tile-title">Register</h3>
			<div class="tile-body">
				<form class="form-horizontal">
					<div class="mb-3 row">
						<label for="text" class="form-label col-md-3">Name</label>
						<div class="col-md-8">
							<input class="form-control" type="text" placeholder="Enter full name" />
						</div>
					</div>
					<div class="mb-3 row">
						<label for="text" class="form-label col-md-3">Email</label>
						<div class="col-md-8">
							<input class="form-control col-md-8" type="email" placeholder="Enter email address" />
						</div>
					</div>
					<div class="mb-3 row">
						<label for="text" class="form-label col-md-3">Address</label>
						<div class="col-md-8">
							<textarea class="form-control" rows="4" placeholder="Enter your address"></textarea>
						</div>
					</div>
					<div class="mb-3 row">
						<label for="text" class="form-label col-md-3">Gender</label>
						<div class="col-md-9">
							<div class="form-check">
								<label class="form-check-label">
									<input class="form-check-input" type="radio" name="gender" />Male
								</label>
							</div>
							<div class="form-check">
								<label class="form-check-label">
									<input class="form-check-input" type="radio" name="gender" />Female
								</label>
							</div>
						</div>
					</div>
					<div class="mb-3 row">
						<label for="text" class="form-label col-md-3">Identity Proof</label>
						<div class="col-md-8">
							<input class="form-control" type="file" />
						</div>
					</div>
					<div class="mb-3 row">
						<div class="col-md-8 col-md-offset-3">
							<div class="form-check">
								<label class="form-check-label">
									<input class="form-check-input" type="checkbox" />I accept the terms and
									conditions
								</label>
							</div>
						</div>
					</div>
				</form>
			</div>
			<div class="tile-footer">
				<div class="row">
					<div class="col-md-8 col-md-offset-3">
						<button class="btn btn-primary" type="button"
							><i class="bi bi-check-circle-fill me-2"></i>Register</button
						>&nbsp;&nbsp;&nbsp;<a class="btn btn-secondary" href="/"
							><i class="bi bi-x-circle-fill me-2"></i>Cancel</a
						>
					</div>
				</div>
			</div>
		</div>
	</div>
	<div class="clearix"></div>
	<div class="col-md-12">
		<div class="tile">
			<h3 class="tile-title">Subscribe</h3>
			<div class="tile-body">
				<form class="row">
					<div class="mb-3 col-md-3">
						<label for="text" class="form-label">Name</label>
						<input class="form-control" type="text" placeholder="Enter your name" />
					</div>
					<div class="mb-3 col-md-3">
						<label for="text" class="form-label">Email</label>
						<input class="form-control" type="text" placeholder="Enter your email" />
					</div>
					<div class="mb-3 col-md-4 align-self-end">
						<button class="btn btn-primary" type="button"
							><i class="bi bi-check-circle-fill me-2"></i>Subscribe</button
						>
					</div>
				</form>
			</div>
		</div>
	</div>
</div>
