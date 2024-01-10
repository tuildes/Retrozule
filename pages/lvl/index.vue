<template>
	<v-container fluid class="wrapper IBMPlex d-flex flex-column align-center">
		<Navbar />
		<!-- Text -->
		<div class="text-content d-flex flex-column text-center">
			<h1>Nada aqui!</h1>
			<v-btn class="mt-1" variant="text" to="/"> Voltar? </v-btn>
		</div>
		<!-- Text -->
	</v-container>
</template>
<script setup>
// Imports
import Navbar from "~/components/global/Navbar.vue"
// Cabeçalhos da pagina
useSeoMeta({
	title: "Retrozule",
	description: "Site experimental de puzzles",
})
useHead({
	htmlAttrs: {
		lang: "pt-br",
	},
	link: [
		{
			rel: "icon",
			type: "image/ico",
			href: "/favicon.ico",
		},
	],
})
</script>
<style scoped>
.wrapper {
	height: 100%;
	width: 100%;
	z-index: 45;
	color: white;
	background: rgb(31, 3, 143);
}

.text-content {
	overflow-y: auto;
	width: 95%;
	gap: 15px;
}
</style>
