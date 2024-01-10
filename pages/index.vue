<template>
	<v-container fluid class="wrapper IBMPlex d-flex flex-column align-center">
		<Navbar />
		<!-- Text -->
		<div class="text-content d-flex flex-column text-center">
			<h1>Bem vindo ao Retrozule!</h1>
			<h3>Esse é um site experimental de "Puzzles"</h3>
			<p>
				Ele é pautado em pequenos desafios de procurar o proximo
				<strong>link</strong> do novo level!
			</p>
			<v-img
				height="15vh"
				alt="Menina de anime na chuva"
				src="https://pa1.aminoapps.com/6861/89c21539c4de40010d44a84040459a2ae3a502f3r1-540-405_hq.gif"
			/>
			<v-btn class="mt-1" variant="text"> Começar? </v-btn>
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
