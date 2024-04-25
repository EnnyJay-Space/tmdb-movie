<template>
	<div class="mb-16">
		<header class="bg-dark-blue">
			<nav class="mx-auto flex max-w-7xl items-center justify-between py-5 " aria-label="Global">
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
						<NuxtLink class="nav-links" to="/"><img class="h-6 w-auto" src="~/assets/images/svgs/plus.svg" alt=""></NuxtLink>
					</div>
					<div>
						<NuxtLink class="nav-links border p-1 rounded text-sm" to="/">EN</NuxtLink>
					</div>
					<div>
						<NuxtLink class="nav-links" to="/">Login</NuxtLink>
					</div>
					<div>
						<NuxtLink class="nav-links" to="/">Join TMDB</NuxtLink>
					</div>
					<div>
						<NuxtLink class="nav-links" to="/"><img class="h-6 w-auto" src="~/assets/images/svgs/search.svg" alt=""></NuxtLink>
					</div>
				</div>
			</nav>
			<!-- Mobile menu, show/hide based on menu open state. -->
		</header>
	</div>
	

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