<template>
	<v-container fluid class="wrapper IBMPlex d-flex flex-column align-center">
		<Navbar />
		<!-- Text -->
		<div class="text-content d-flex flex-column text-center">
			<h3>Soluções</h3>
			<details v-for="(item, i) in levels" :key="i">
				<summary>{{ item.title }}</summary>
				{{ item.text }}
			</details>
			<v-btn class="mt-1" variant="text" to="/"> Voltar? </v-btn>
		</div>
		<!-- Text -->
	</v-container>
</template>
<script setup>
// Imports
import Navbar from "~/components/global/Navbar.vue"

const levels = [
	{
		title: "Introdução",
		text: "Como a fase diz, basta ir para o url da primeira fase [ ../lvl/level-um ]",
	},
	{
		title: "Level 1",
		text: "Basta selecionar todo o espaço vazio do gif, e copiar o texto que aparece",
	},
	{
		title: "Level 2",
		text: "Pesquisa a música e veja o verso que está faltando no espaço vazio",
	},
	{
		title: "Level 3",
		text: "Na imagem existe um numero escondido em branco, coloque esse numero e clique em enviar. Feito isso veja o titulo da fase",
	},
	{
		title: "Level 4",
		text: "Clique as músicas em ordem do álbum bittersweet memories e veja a frase que será feita",
	},
	{
		title: "Level 5",
		text: "Clique em trocar música até aparecer um áudio de morse, decode o áudio e veja a frase que será feita",
	},
]

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
