<script>
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
	<header>
		<div class="wrapper">
			<nav>
				<RouterLink to="/">Home</RouterLink>
				<RouterLink to="/CategoryView">Categories</RouterLink>
				<RouterLink to="/Breakdowns">Breakdowns</RouterLink>
				<RouterLink to="/about">About</RouterLink>
			</nav>
		</div>
	</header>

	<RouterView />
</template>

<style scoped>
nav {
	width: 100%;
	font-size: 12px;
	text-align: center;
}

nav a.router-link-exact-active {
	color: var(--color-text);
}

nav a.router-link-exact-active:hover {
	background-color: transparent;
}

nav a {
	display: inline-block;
	padding: 0 1rem;
	border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
	border: 0;
}
</style>
