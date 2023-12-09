<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'

</script>

<template>
	<header>
		<div>
		</div>
		<div id="routers">
			<div class="router_up">
				<RouterLink class="router" to="/">Home</RouterLink>
			</div>
			<div class="router_up">
				<RouterLink class="router" to="/about">About</RouterLink>
			</div>
			<div class="router_up">
				<RouterLink class="router" to="/links">Links</RouterLink>
			</div>
		</div>
		<div>
		</div>
	</header>
	<div id="routerView">
		<RouterView />
	</div>
</template>

<style scoped>
header {
	margin-top: 1vh;
	width: 100%;
	display: flex;
	align-items: center;
	justify-content: space-between;
}

#routerView {
	margin-top: 1vh;
}

#routers {
	display: flex;
	align-items: center;
	background-color: var(--dark3);
	padding: 0.25vw;
	border-radius: 1vw;
	filter: drop-shadow(0.5vw 0.5vh 0.25vw #090909);
}

.router_up {
	transition: all 0.05s ease-out;
	background-color: var(--dark2);
	border-radius: 0.75vw;
	display: flex;
	align-items: center;
	justify-content: center;
	padding: 0 3vw;
	margin: 0 0.25vw;
}

.router_up:hover {
	background-color: var(--dark1);
	padding: 0 3.25vw;
	filter: drop-shadow(0 0 0.5rem rgb(14, 14, 14));
}

.router_up:active {
	filter: drop-shadow(0 0 0.75rem crimson);
	background-color: crimson;
	padding: 0 2.5vw;
}

.router {
	margin: 0.25vw;
}

h1 {
	font-family: 'Fraunces', serif;
}

@media only screen and (max-width: 600px) {
	.router_up {
		margin: 1vw 1vw;
		border-radius: 1vh;
	}

	.router {
		margin: 1vh;
	}
}
</style>