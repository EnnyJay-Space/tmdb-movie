<template>
	<div class="mb-16">
		<header class="bg-dark-blue">
			<nav class="mx-auto flex max-w-7xl items-center justify-between p-5 lg:px-8" aria-label="Global">
				<div class="flex">
					<a href="#" class="-m-1.5 p-1.5">
						<img class="h-6 w-auto" src="~/assets/images/svgs/logo.svg" alt="">
					</a>
				</div>
				<div class="flex lg:hidden">
					<button type="button" class="-m-2.5 inline-flex items-center justify-center rounded-md p-2.5 text-gray-700">
						<svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor"
							aria-hidden="true">
							<path stroke-linecap="round" stroke-linejoin="round" d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5" />
						</svg>
					</button>
				</div>

				<div class="hidden lg:flex lg:gap-x-8 justify-center ms-5">
					<div class="dropdown">
						<NuxtLink class="dropbtn nav-links">Movies</NuxtLink>
						<div class="dropdown-content">
							<NuxtLink class="dropdown-links" to="/">Popular</NuxtLink>
							<NuxtLink class="dropdown-links" to="/">Now Playing</NuxtLink>
							<NuxtLink class="dropdown-links" to="/">Upcoming</NuxtLink>
							<NuxtLink class="dropdown-links" to="/">Top Rated</NuxtLink>
						</div>
					</div>
					<div class="dropdown">
						<NuxtLink class="dropbtn nav-links">TV Shows</NuxtLink>
						<div class="dropdown-content">
							<NuxtLink class="dropdown-links" to="/">Popular</NuxtLink>
							<NuxtLink class="dropdown-links" to="/">Airing Today</NuxtLink>
							<NuxtLink class="dropdown-links" to="/">On TV</NuxtLink>
							<NuxtLink class="dropdown-links" to="/">Top Rated</NuxtLink>
						</div>
					</div>
					<div class="dropdown">
						<NuxtLink class="dropbtn nav-links">People</NuxtLink>
						<div class="dropdown-content">
							<NuxtLink class="dropdown-links" to="/">Popular People</NuxtLink>
						</div>
					</div>
					<div class="dropdown">
						<NuxtLink class="dropbtn nav-links">More</NuxtLink>
						<div class="dropdown-content">
							<NuxtLink class="dropdown-links" to="/">Discussion</NuxtLink>
							<NuxtLink class="dropdown-links" to="/">Leaderboard</NuxtLink>
							<NuxtLink class="dropdown-links" to="/">Support</NuxtLink>
							<NuxtLink class="dropdown-links" to="/">API</NuxtLink>
						</div>
					</div>




				</div>
				<div class="hidden lg:flex lg:flex-1 lg:gap-x-8 lg:justify-end">
					<div>
						<NuxtLink class="nav-links" to="/">EN</NuxtLink>
					</div>
					<div>
						<NuxtLink class="nav-links" to="/">Login</NuxtLink>
					</div>
					<div>
						<NuxtLink class="nav-links" to="/">Join TMDB</NuxtLink>
					</div>
					<div>
						<!-- <img class="h-6 w-auto" src="~/assets/images/svgs/search.svg" alt=""> -->
						<NuxtLink class="nav-links" to="/"><img class="h-6 w-auto" src="~/assets/images/svgs/search.png" alt=""></NuxtLink>
					</div>
				</div>
			</nav>
			<!-- Mobile menu, show/hide based on menu open state. -->

		</header>

	</div>
	<nav class="bg-gray-800">
		<div class="mx-auto max-w-7xl px-2 sm:px-6 lg:px-8">
			<div class="relative flex h-16 items-center justify-between">
				<div class="absolute inset-y-0 left-0 flex items-center sm:hidden">
					<!-- Mobile menu button-->
					<button type="button"
						class="relative inline-flex items-center justify-center rounded-md p-2 text-gray-400 hover:bg-gray-700 hover:text-white focus:outline-none focus:ring-2 focus:ring-inset focus:ring-white"
						aria-controls="mobile-menu" aria-expanded="false">
						<span class="absolute -inset-0.5"></span>
						<span class="sr-only">Open main menu</span>
						<!--
            Icon when menu is closed.

            Menu open: "hidden", Menu closed: "block"
          -->
						<svg class="block h-6 w-6" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor"
							aria-hidden="true">
							<path stroke-linecap="round" stroke-linejoin="round" d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5" />
						</svg>
						<!--
            Icon when menu is open.

            Menu open: "block", Menu closed: "hidden"
          -->
						<svg class="hidden h-6 w-6" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor"
							aria-hidden="true">
							<path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12" />
						</svg>
					</button>
				</div>
				<div class="flex flex-1 items-center justify-center sm:items-stretch sm:justify-start">
					<div class="flex flex-shrink-0 items-center">
						<img class="h-8 w-auto" src="https://tailwindui.com/img/logos/mark.svg?color=indigo&shade=500"
							alt="Your Company">
					</div>
					<div class="hidden sm:ml-6 sm:block">
						<div class="flex space-x-4">
							<!-- Current: "bg-gray-900 text-white", Default: "text-gray-300 hover:bg-gray-700 hover:text-white" -->
							<a href="#" class="bg-gray-900 text-white rounded-md px-3 py-2 text-sm font-medium"
								aria-current="page">Dashboard</a>
							<a href="#"
								class="text-gray-300 hover:bg-gray-700 hover:text-white rounded-md px-3 py-2 text-sm font-medium">Team</a>
							<a href="#"
								class="text-gray-300 hover:bg-gray-700 hover:text-white rounded-md px-3 py-2 text-sm font-medium">Projects</a>
							<a href="#"
								class="text-gray-300 hover:bg-gray-700 hover:text-white rounded-md px-3 py-2 text-sm font-medium">Calendar</a>
						</div>
					</div>
				</div>
				<div class="absolute inset-y-0 right-0 flex items-center pr-2 sm:static sm:inset-auto sm:ml-6 sm:pr-0">
					<button type="button"
						class="relative rounded-full bg-gray-800 p-1 text-gray-400 hover:text-white focus:outline-none focus:ring-2 focus:ring-white focus:ring-offset-2 focus:ring-offset-gray-800">
						<span class="absolute -inset-1.5"></span>
						<svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor"
							aria-hidden="true">
							<path stroke-linecap="round" stroke-linejoin="round"
								d="M14.857 17.082a23.848 23.848 0 005.454-1.31A8.967 8.967 0 0118 9.75v-.7V9A6 6 0 006 9v.75a8.967 8.967 0 01-2.312 6.022c1.733.64 3.56 1.085 5.455 1.31m5.714 0a24.255 24.255 0 01-5.714 0m5.714 0a3 3 0 11-5.714 0" />
						</svg>
					</button>

					<!-- Profile dropdown -->
					<!--  -->
				</div>
			</div>
		</div>

		<!-- Mobile menu, show/hide based on menu state. -->
		<div class="sm:hidden" id="mobile-menu">
			<div class="space-y-1 px-2 pb-3 pt-2">
				<!-- Current: "bg-gray-900 text-white", Default: "text-gray-300 hover:bg-gray-700 hover:text-white" -->
				<a href="#" class="bg-gray-900 text-white block rounded-md px-3 py-2 text-base font-medium"
					aria-current="page">Dashboard</a>
				<a href="#"
					class="text-gray-300 hover:bg-gray-700 hover:text-white block rounded-md px-3 py-2 text-base font-medium">Team</a>
				<a href="#"
					class="text-gray-300 hover:bg-gray-700 hover:text-white block rounded-md px-3 py-2 text-base font-medium">Projects</a>
				<a href="#"
					class="text-gray-300 hover:bg-gray-700 hover:text-white block rounded-md px-3 py-2 text-base font-medium">Calendar</a>
			</div>
		</div>
	</nav>

</template>

<script>
export default {

}
</script>

<style scoped>
/* NAVBAR CSS */
.nav-links {
	color: #ffffff;
	font-weight: 600;
}



/* BACKGROUND COLORS*/
.bg-dark-blue {
	background-color: #032541;
}



/* NAVBAR DROPDOWN CSS */
.dropdown {
	position: relative;
	display: inline-block;
}

.dropdown-content {
	border-radius: 5px;
	display: none;
	position: absolute;
	background-color: #ffffff;
	min-width: 160px;
	box-shadow: 0px 8px 16px 0px rgba(0, 0, 0, 0.2);
	z-index: 1;
}

.dropdown-content .dropdown-links {
	color: black;
	padding: 5px 16px;
	text-decoration: none;
	display: block;
}

.dropdown-content .dropdown-links:hover {
	color: black;
	padding: 5px 16px;
	text-decoration: none;
	background-color: #f1f1f1;
	display: block;
}

.dropdown:hover .dropdown-content {
	display: block;
}
</style>