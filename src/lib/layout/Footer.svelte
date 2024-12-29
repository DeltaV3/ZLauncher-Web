<script>

	const footerNavs = [
		{
			label: 'En esta pagina',
			items: [
				// {
				// 	href: '/',
				// 	name: 'Email Collection'
				// },
				{
					href: '#pricing',
					name: 'Precio'
				}
				// {
				// 	href: '/faq',
				// 	name: 'FAQ'
				// }
			]
		},

		{
			label: 'Comunidad',
			items: [
				{
					href: 'https://github.com/DeltaV3/ZLauncher',
					name: 'Github'
				},
				{
					href: 'https://discord.com/invite/vHCbvhzrj5',
					name: 'Discord'
				}	
			]
		},
		{
			label: 'Legal',
			items: [
				{
					href: 'https://github.com/DeltaV3/ZLauncher/blob/master/LICENSE.txt',
					name: 'Licencia'
				}
			]
		}
	];

	const footerSocials = [
		{
			href: 'https://github.com/DeltaV3/Zlauncher',
			name: 'Github',
			icon: 'data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxZW0iIGhlaWdodD0iMWVtIiB2aWV3Qm94PSIwIDAgMjQgMjQiPjxwYXRoIGZpbGw9IiNmZmZmZmYiIGQ9Ik0xMiAyQTEwIDEwIDAgMCAwIDIgMTJjMCA0LjQyIDIuODcgOC4xNyA2Ljg0IDkuNWMuNS4wOC42Ni0uMjMuNjYtLjV2LTEuNjljLTIuNzcuNi0zLjM2LTEuMzQtMy4zNi0xLjM0Yy0uNDYtMS4xNi0xLjExLTEuNDctMS4xMS0xLjQ3Yy0uOTEtLjYyLjA3LS42LjA3LS42YzEgLjA3IDEuNTMgMS4wMyAxLjUzIDEuMDNjLjg3IDEuNTIgMi4zNCAxLjA3IDIuOTEuODNjLjA5LS42NS4zNS0xLjA5LjYzLTEuMzRjLTIuMjItLjI1LTQuNTUtMS4xMS00LjU1LTQuOTJjMC0xLjExLjM4LTIgMS4wMy0yLjcxYy0uMS0uMjUtLjQ1LTEuMjkuMS0yLjY0YzAgMCAuODQtLjI3IDIuNzUgMS4wMmMuNzktLjIyIDEuNjUtLjMzIDIuNS0uMzNzMS43MS4xMSAyLjUuMzNjMS45MS0xLjI5IDIuNzUtMS4wMiAyLjc1LTEuMDJjLjU1IDEuMzUuMiAyLjM5LjEgMi42NGMuNjUuNzEgMS4wMyAxLjYgMS4wMyAyLjcxYzAgMy44Mi0yLjM0IDQuNjYtNC41NyA0LjkxYy4zNi4zMS42OS45Mi42OSAxLjg1VjIxYzAgLjI3LjE2LjU5LjY3LjVDMTkuMTQgMjAuMTYgMjIgMTYuNDIgMjIgMTJBMTAgMTAgMCAwIDAgMTIgMiIvPjwvc3ZnPg=='
		}
	];
</script>

<footer>
	<div class="mx-auto w-full max-w-screen-xl xl:pb-2">
		<div class="gap-4 p-4 px-8 py-16 sm:pb-16 md:flex md:justify-between">
			<div class="mb-12 flex flex-col gap-4">
				<a href="/" class="flex items-center gap-2">
					<img src="http://techterra.x10.mx/minecraft_title.png" alt="logo" class="h-8 w-auto" />

				</a>
				<p class="max-w-xs">Instala Minecraft, Java, Forge y los mods del servidor con facilidad.</p>
			</div>
			<div class="grid grid-cols-1 gap-8 sm:grid-cols-3 sm:gap-10">
				{#each footerNavs as nav}
					<div>
						<h2
							class="mb-6 text-sm font-medium uppercase tracking-tighter text-gray-900 dark:text-white"
						>
							{nav.label}
						</h2>
						<ul class="grid gap-2">
							{#each nav.items as item}
								<li>
									<a
										href={item.href}
										class="cursor-pointer text-sm font-[450] text-gray-400 duration-200 hover:text-gray-200"
									>
										{item.name}
									</a>
								</li>
							{/each}
						</ul>
					</div>
				{/each}
			</div>
		</div>

		<div
			class="flex flex-col gap-2 rounded-md border-neutral-700/20 px-8 py-4 sm:flex sm:flex-row sm:items-center sm:justify-between"
		>
			<div class="flex items-center space-x-5 sm:mt-0 sm:justify-center">
				{#each footerSocials as social}
					<a
						href={social.href}
						class="fill-gray-500 text-gray-500 hover:fill-gray-900 hover:text-gray-900 dark:hover:fill-gray-600 dark:hover:text-gray-600"
					>
						<img src={social.icon} class="size-7" alt={social.name} />
						<span class="sr-only">{social.name}</span>
					</a>
				{/each}
			</div>
			<span class="text-sm text-gray-500 dark:text-gray-400 sm:text-center">
				Copyright ©
				{' '}
				{new Date().getFullYear()}
				{' '}
				<a href="/" class="cursor-pointer">ZLauncher</a>. All Rights Reserved.
			</span>
		</div>
	</div>
	<!-- Site Banner -->
</footer>
