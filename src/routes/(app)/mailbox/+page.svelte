<script>
	import AppTitle from '$lib/components/AppTitle.svelte';
</script>

<svelte:head>
	<title>Mailbox - Vali Admin</title>
</svelte:head>

<AppTitle title="Mailbox" desc="A Mailbox page sample" iconTitle="bi bi-envelope-at" />

<div class="row">
	<div class="col-md-3">
		<div class="d-grid"><a class="mb-2 btn btn-primary btn-block" href="/">Compose Mail</a></div>
		<div class="tile p-0">
			<h4 class="tile-title folder-head">Folders</h4>
			<div class="tile-body">
				<ul class="nav nav-pills flex-column mail-nav">
					<li class="nav-item">
						<a class="nav-link d-flex justify-content-between align-items-start" href="/"
							><span><i class="bi bi-inbox me-1 fs-5"></i> Inbox</span><span
								class="badge bg-primary rounded-pill">12</span
							></a
						>
					</li>
					<li class="nav-item">
						<a class="nav-link" href="/"><i class="bi bi-envelope me-1 fs-5"></i> Sent</a>
					</li>
					<li class="nav-item">
						<a class="nav-link" href="/"><i class="bi bi-journal-text me-1 fs-5"></i> Drafts</a>
					</li>
					<li class="nav-item">
						<a class="nav-link d-flex justify-content-between align-items-start" href="/"
							><span><i class="bi bi-funnel me-1 fs-5"></i> Junk </span><span
								class="badge bg-primary rounded-pill">8</span
							></a
						>
					</li>
					<li class="nav-item">
						<a class="nav-link" href="/"><i class="bi bi-trash me-1 fs-5"></i> Trash</a>
					</li>
				</ul>
			</div>
		</div>
	</div>
	<div class="col-md-9">
		<div class="tile">
			<div class="mailbox-controls">
				<div class="form-check">
					<label>
						<input class="form-check-input" type="checkbox" /><span class="label-text"></span>
					</label>
				</div>
				<div class="btn-group">
					<button class="btn btn-primary btn-sm" type="button"
						><i class="bi bi-trash fs-5"></i></button
					>
					<button class="btn btn-primary btn-sm" type="button"
						><i class="bi bi-reply fs-5"></i></button
					>
					<button class="btn btn-primary btn-sm" type="button"
						><i class="bi bi-share fs-5"></i></button
					>
					<button class="btn btn-primary btn-sm" type="button"
						><i class="bi bi-arrow-clockwise fs-5"></i></button
					>
				</div>
			</div>
			<div class="table-responsive mailbox-messages">
				<!-- svelte-ignore a11y-invalid-attribute -->
				<table class="table table-hover">
					<tbody>
						<tr>
							<td>
								<div class="form-check">
									<label>
										<input class="form-check-input" type="checkbox" /><span class="label-text">
										</span>
									</label>
								</div>
							</td>
							<td><a href="#" on:click|preventDefault><i class="bi bi-star"></i></a></td>
							<td><a href="read-mail.html">John Doe</a></td>
							<td class="mail-subject"
								><b>A report on project almanac</b> - Lorem ipsum dolor sit amet adipisicing elit...</td
							>
							<td><i class="bi bi-paperclip"></i></td>
							<td>8 mins ago</td>
						</tr>
						<tr>
							<td>
								<div class="form-check">
									<label>
										<input class="form-check-input" type="checkbox" /><span class="label-text">
										</span>
									</label>
								</div>
							</td>
							<td><a href="#" on:click|preventDefault><i class="bi bi-star-fill"></i></a></td>
							<td><a href="read-mail.html">John Doe</a></td>
							<td
								><b>A report on some good project</b> - Lorem ipsum dolor sit amet adipisicing elit...</td
							>
							<td></td>
							<td>15 mins ago</td>
						</tr>
						<tr>
							<td>
								<div class="form-check">
									<label>
										<input class="form-check-input" type="checkbox" /><span class="label-text">
										</span>
									</label>
								</div>
							</td>
							<td><a href="#" on:click|preventDefault><i class="bi bi-star"></i></a></td>
							<td><a href="read-mail.html">John Doe</a></td>
							<td class="mail-subject"
								><b>A report on project almanac</b> - Lorem ipsum dolor sit amet adipisicing elit...</td
							>
							<td><i class="bi bi-paperclip"></i></td>
							<td>30 mins ago</td>
						</tr>
						<tr>
							<td>
								<div class="form-check">
									<label>
										<input class="form-check-input" type="checkbox" /><span class="label-text">
										</span>
									</label>
								</div>
							</td>
							<td><a href="#" on:click|preventDefault><i class="bi bi-star-fill"></i></a></td>
							<td><a href="read-mail.html">John Doe</a></td>
							<td class="mail-subject"
								><b>A report on project almanac</b> - Lorem ipsum dolor sit amet adipisicing elit...</td
							>
							<td></td>
							<td>25 December</td>
						</tr>
						<tr>
							<td>
								<div class="form-check">
									<label>
										<input class="form-check-input" type="checkbox" /><span class="label-text">
										</span>
									</label>
								</div>
							</td>
							<td><a href="#" on:click|preventDefault><i class="bi bi-star"></i></a></td>
							<td><a href="read-mail.html">John Doe</a></td>
							<td class="mail-subject"
								><b>A report on project almanac</b> - Lorem ipsum dolor sit amet adipisicing elit...</td
							>
							<td><i class="bi bi-paperclip"></i></td>
							<td>20 December</td>
						</tr>
						<tr>
							<td>
								<div class="form-check">
									<label>
										<input class="form-check-input" type="checkbox" /><span class="label-text">
										</span>
									</label>
								</div>
							</td>
							<td><a href="#" on:click|preventDefault><i class="bi bi-star-fill"></i></a></td>
							<td><a href="read-mail.html">John Doe</a></td>
							<td class="mail-subject"
								><b>A report on project almanac</b> - Lorem ipsum dolor sit amet adipisicing elit...</td
							>
							<td></td>
							<td>20 December</td>
						</tr>
						<tr>
							<td>
								<div class="form-check">
									<label>
										<input class="form-check-input" type="checkbox" /><span class="label-text">
										</span>
									</label>
								</div>
							</td>
							<td><a href="#" on:click|preventDefault><i class="bi bi-star-fill"></i></a></td>
							<td><a href="read-mail.html">John Doe</a></td>
							<td class="mail-subject"
								><b>A report on project almanac</b> - Lorem ipsum dolor sit amet adipisicing elit...</td
							>
							<td><i class="bi bi-paperclip"></i></td>
							<td>20 December</td>
						</tr>
						<tr>
							<td>
								<div class="form-check">
									<label>
										<input class="form-check-input" type="checkbox" /><span class="label-text">
										</span>
									</label>
								</div>
							</td>
							<td><a href="#" on:click|preventDefault><i class="bi bi-star"></i></a></td>
							<td><a href="read-mail.html">John Doe</a></td>
							<td class="mail-subject"
								><b>A report on project almanac</b> - Lorem ipsum dolor sit amet adipisicing elit...</td
							>
							<td></td>
							<td>20 December</td>
						</tr>
					</tbody>
				</table>
			</div>
			<div class="text-end">
				<span class="text-muted mr-2">Showing 1-15 out of 60</span>
				<div class="btn-group ms-3">
					<button class="btn btn-primary btn-sm" type="button"
						><i class="bi bi-chevron-left"></i></button
					>
					<button class="btn btn-primary btn-sm" type="button"
						><i class="bi bi-chevron-right"></i></button
					>
				</div>
			</div>
		</div>
	</div>
</div>
