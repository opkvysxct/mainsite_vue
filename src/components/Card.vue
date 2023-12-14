<script setup lang="ts">

</script>

<template>
	<div id="card">
		<div id="img_div">
			<img src="../../public/cards/1.png" alt="card">
		</div>
		<h1>Title</h1>
		<p>Duis elit aute laborum esse officia nulla velit nisi enim irure occaecat adipisicing.</p>
	</div>
</template>

<style scoped>
img {
	object-fit: cover;
	width: 100%;
}

#img_div {
	display: flex;
	overflow: hidden;
	border-radius: 0.25vw;
	height: 30vh;
	width: 15vw;
}

h1 {
	margin: 0.5vw;
}

p {
	margin: 0.25vw;
	color: var(--light2);
}

#card {
	overflow: hidden;
	border-radius: 0.5vw;
	width: 15vw;
	height: 35vh;
	background-color: var(--dark2);
	display: flex;
	flex-direction: column;
	align-items: center;
	justify-content: center;
	filter: drop-shadow(0.5vw 0.5vh 0.25vw #090909);
}
</style>