<script>
	import { page } from '$app/stores';
	import { onMount } from 'svelte';

	// Fungsi untuk memeriksa apakah suatu elemen menu aktif
	let isActive = $derived((/** @type {any} */ item) => {
		const currentPath = $page.url.pathname;
		return (
			item.link === currentPath ||
			(item.submenu &&
				item.submenu.some(
					(/** @type {{ link: string; }} */ subitem) => subitem.link === currentPath
				))
		);
	});

	const dataMenu = [
		{
			label: 'Dashboard',
			icon: 'bi bi-speedometer',
			link: '/'
		},
		{
			label: 'UI Elements',
			icon: 'bi bi-laptop',
			submenu: [
				{
					label: 'Bootstrap Elements',
					icon: 'bi bi-circle-fill',
					link: '/bootstrap-components'
				},
				{
					label: 'Font Icons',
					icon: 'bi bi-circle-fill',
					link: 'https://icons.getbootstrap.com/',
					target: '_blank',
					rel: 'noopener'
				},
				{
					label: 'Cards',
					icon: 'bi bi-circle-fill',
					link: '/cards'
				},
				{
					label: 'Widgets',
					icon: 'bi bi-circle-fill',
					link: '/widgets'
				}
			]
		},
		{
			label: 'Forms',
			icon: 'bi bi-ui-checks',
			submenu: [
				{
					label: 'Form Components',
					icon: 'bi bi-circle-fill',
					link: '/form-components'
				},
				{
					label: 'Form Samples',
					icon: 'bi bi-circle-fill',
					link: '/form-samples'
				}
			]
		},
		{
			label: 'Tables',
			icon: 'bi bi-table',
			submenu: [
				{
					label: 'Basic Tables',
					icon: 'bi bi-circle-fill',
					link: '/table-basic'
				},
				{
					label: 'Data Tables',
					icon: 'bi bi-circle-fill',
					link: '/datatable'
				}
			]
		},
		{
			label: 'Pages',
			icon: 'bi bi-file-earmark',
			submenu: [
				{
					label: 'Blank Page',
					icon: 'bi bi-circle-fill',
					link: '/blank'
				},
				{
					label: 'Login Page',
					icon: 'bi bi-circle-fill',
					link: '/login'
				},
				{
					label: 'Lockscreen Page',
					icon: 'bi bi-circle-fill',
					link: '/lockscreen'
				},
				{
					label: 'User Page',
					icon: 'bi bi-circle-fill',
					link: '/user'
				},
				{
					label: 'Invoice Page',
					icon: 'bi bi-circle-fill',
					link: '/invoice'
				},
				{
					label: 'Mailbox',
					icon: 'bi bi-circle-fill',
					link: '/mailbox'
				},
				{
					label: 'Error Page',
					icon: 'bi bi-circle-fill',
					link: '/error'
				}
			]
		},
		{
			label: 'Docs',
			icon: 'bi bi-code-square',
			link: '/docs'
		}
	];

	onMount(async () => {
		const treeviewMenu = document.querySelector('.app-menu');

		// Toggle Sidebar
		// @ts-ignore
		document.querySelector('[data-toggle="sidebar"]').addEventListener('click', function (event) {
			event.preventDefault();
			// @ts-ignore
			document.querySelector('.app').classList.toggle('sidenav-toggled');
		});

		// Activate sidebar treeview toggle
		const treeviewToggleElements = document.querySelectorAll("[data-toggle='treeview']");
		treeviewToggleElements.forEach(function (element) {
			element.addEventListener('click', function (event) {
				event.preventDefault();
				const parentElement = element.parentElement;

				// @ts-ignore
				if (!parentElement.classList.contains('is-expanded')) {
					// @ts-ignore
					var allTreeViewElements = treeviewMenu.querySelectorAll("[data-toggle='treeview']");
					allTreeViewElements.forEach(function (treeviewElement) {
						// @ts-ignore
						treeviewElement.parentElement.classList.remove('is-expanded');
					});
				}

				// @ts-ignore
				parentElement.classList.toggle('is-expanded');
			});
		});
	});
</script>

<div class="app-sidebar__overlay" data-toggle="sidebar"></div>
<aside class="app-sidebar">
	<div class="app-sidebar__user">
		<img
			class="app-sidebar__user-avatar"
			src="https://randomuser.me/api/portraits/men/1.jpg"
			alt="User"
		/>
		<div>
			<p class="app-sidebar__user-name">John Doe</p>
			<p class="app-sidebar__user-designation">Frontend Developer</p>
		</div>
	</div>
	<!-- svelte-ignore a11y_invalid_attribute -->
	<ul class="app-menu">
		{#each dataMenu as item (item.label)}
			{#if item.submenu}
				<div class={isActive(item) ? 'treeview is-expanded' : 'treeview'}>
					<a class="app-menu__item" href="#" data-toggle="treeview">
						<i class="app-menu__icon {item.icon}"></i>
						<span class="app-menu__label">{item.label}</span>
						<i class="treeview-indicator bi bi-chevron-right"></i>
					</a>
					<ul class="treeview-menu">
						{#each item.submenu as subitem (subitem.label)}
							<li>
								<a
									class={isActive(subitem) ? 'treeview-item active' : 'treeview-item'}
									href={subitem.link}
									target={subitem.target}
									rel={subitem.rel}
								>
									<i class="icon {subitem.icon}"></i>
									{subitem.label}
								</a>
							</li>
						{/each}
					</ul>
				</div>
			{:else}
				<a class={isActive(item) ? 'app-menu__item active' : 'app-menu__item'} href={item.link}>
					<i class="app-menu__icon {item.icon}"></i>
					<span class="app-menu__label">{item.label}</span>
				</a>
			{/if}
		{/each}
	</ul>
</aside>
