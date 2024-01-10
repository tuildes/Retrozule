<template>
	<div class="wrapper d-flex align-center px-4 mb-4">
		<a href="https://github.com/tuildes" class="title">TUILDES</a>
		<v-spacer />
		<div class="d-flex link">
			<nuxt-link to="/" class="link">Home</nuxt-link>
			&diams;
			<nuxt-link to="/help" class="link">Help</nuxt-link>
		</div>
	</div>
</template>
<script setup></script>
<style scoped>
.wrapper {
	width: 100%;
	height: min-content !important;
}

.title {
	font-family: "FZNDGrana", Arial, sans-serif;
	font-size: 30px;
	text-decoration: none;
	color: white;
	font-weight: 800;
}

.link {
	color: white;
	text-decoration: none;
	font-weight: 800;
	gap: 10px;
}
</style>
