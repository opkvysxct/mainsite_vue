<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import icon_home from "./icons/icon_home.vue"
import icon_about from "./icons/icon_about.vue"
import icon_links from "./icons/icon_links.vue"
</script>

<template>
	<header>
		<div>
			<h1>VYSX</h1>
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
			<h1>VYSX</h1>
		</div>
	</header>
	<RouterView />
</template>

<style scoped>
header {
	margin-top: 1vh;
	width: 100%;
	display: flex;
	align-items: center;
	justify-content: space-between;
}

#routers {
	display: flex;
	align-items: center;
	background-color: var(--dark3);
	padding: 0.25vw;
	border-radius: 0.25vw;
}

.router_up {
	transition: all 0.05s ease-out;
	background-color: var(--dark2);
	border-radius: 0.5vw;
	display: flex;
	align-items: center;
	justify-content: center;
	padding: 0 2vw;
	margin: 0 0.25vw;
}

.router_up:hover {
	background-color: var(--dark1);
	padding: 0 2.25vw;
}

.router_up:active {
	background-color: var(--accent1);
	padding: 0 2vw;
}

.router {
	margin: 0.25vw;
}

h1 {
	font-family: 'Fraunces', serif;
}
</style>