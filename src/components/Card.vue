<script setup lang="ts">

</script>

<template>
	<div id="card">
		<img src="../../public/cards/1.png" alt="card">
		<p>something</p>
	</div>
</template>

<style scoped>
img {
	width: 15vw;
	margin: 1vw;
	border-radius: 0.25vw;
}

p {
	font-size: 1.5vw;
	margin-bottom: 1vw;
}

#card {
	border-radius: 0.75vw;
	width: 15vw;
	background-color: var(--dark2);
	display: flex;
	flex-direction: column;
	align-items: center;
	justify-content: center;
	filter: drop-shadow(0.5vw 0.5vh 0.25vw #090909);
}
</style>