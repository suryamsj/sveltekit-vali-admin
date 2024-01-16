<svelte:head>
	<title>User Profile - Vali Admin</title>
</svelte:head>

<div class="row user">
	<div class="col-md-12">
		<div class="profile">
			<div class="info">
				<img class="user-img" src="https://randomuser.me/api/portraits/men/1.jpg" alt="Men" />
				<h4>John Doe</h4>
				<p>FrontEnd Developer</p>
			</div>
			<div class="cover-image"></div>
		</div>
	</div>
	<div class="col-md-3">
		<div class="tile p-0">
			<ul class="nav flex-column nav-tabs user-tabs">
				<li class="nav-item">
					<a class="nav-link active" href="#user-timeline" data-bs-toggle="tab">Timeline</a>
				</li>
				<li class="nav-item">
					<a class="nav-link" href="#user-settings" data-bs-toggle="tab">Settings</a>
				</li>
			</ul>
		</div>
	</div>
	<div class="col-md-9">
		<div class="tab-content">
			<div class="tab-pane active" id="user-timeline">
				<div class="timeline-post">
					<div class="post-media">
						<a href="/"><img src="https://randomuser.me/api/portraits/men/1.jpg" alt="Men" /></a>
						<div class="content">
							<h5><a href="/">John Doe</a></h5>
							<p class="text-muted"><small>2 January at 9:30</small></p>
						</div>
					</div>
					<div class="post-content">
						<p>
							Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor
							incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis tion
							ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in
							reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
							Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt
							mollit anim id est laborum.
						</p>
					</div>
					<ul class="post-utility">
						<li class="likes"><a href="/"><i class="bi bi-heart me-1"></i>Like</a></li>
						<li class="shares"><a href="/"><i class="bi bi-share me-1"></i>Share</a></li>
						<li class="comments"><i class="bi bi-chat-square-text me-1"></i> 5 Comments</li>
					</ul>
				</div>
				<div class="timeline-post">
					<div class="post-media">
						<a href="/"><img src="https://randomuser.me/api/portraits/men/1.jpg" alt="Men" /></a>
						<div class="content">
							<h5><a href="/">John Doe</a></h5>
							<p class="text-muted"><small>2 January at 9:30</small></p>
						</div>
					</div>
					<div class="post-content">
						<p>
							Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor
							incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis tion
							ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in
							reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
							Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt
							mollit anim id est laborum.
						</p>
					</div>
					<ul class="post-utility">
						<li class="likes"><a href="/"><i class="bi bi-heart me-1"></i>Like</a></li>
						<li class="shares"><a href="/"><i class="bi bi-share me-1"></i>Share</a></li>
						<li class="comments"><i class="bi bi-chat-square-text me-1"></i> 5 Comments</li>
					</ul>
				</div>
			</div>
			<div class="tab-pane fade" id="user-settings">
				<div class="tile user-settings">
					<h4 class="line-head">Settings</h4>
					<form>
						<div class="row mb-4">
							<div class="col-md-4">
								<label for="text">First Name</label>
								<input class="form-control" type="text" />
							</div>
							<div class="col-md-4">
								<label for="text">Last Name</label>
								<input class="form-control" type="text" />
							</div>
						</div>
						<div class="row">
							<div class="col-md-8 mb-4">
								<label for="text">Email</label>
								<input class="form-control" type="text" />
							</div>
							<div class="clearfix"></div>
							<div class="col-md-8 mb-4">
								<label for="text">Mobile No</label>
								<input class="form-control" type="text" />
							</div>
							<div class="clearfix"></div>
							<div class="col-md-8 mb-4">
								<label for="text">Office Phone</label>
								<input class="form-control" type="text" />
							</div>
							<div class="clearfix"></div>
							<div class="col-md-8 mb-4">
								<label for="text">Home Phone</label>
								<input class="form-control" type="text" />
							</div>
						</div>
						<div class="row mb-10">
							<div class="col-md-12">
								<button class="btn btn-primary" type="button"
									><i class="bi bi-check-circle-fill me-2"></i> Save</button
								>
							</div>
						</div>
					</form>
				</div>
			</div>
		</div>
	</div>
</div>
