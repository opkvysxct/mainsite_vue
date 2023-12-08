<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'

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
}

.router_up:active {
	background-color: var(--accent1);
	padding: 0 3vw;
}

.router {
	margin: 0.25vw;
}

h1 {
	font-family: 'Fraunces', serif;
}
</style>