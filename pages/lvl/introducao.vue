<template>
	<v-container fluid class="wrapper IBMPlex d-flex flex-column align-center">
		<!-- Text -->
		<div class="text-content d-flex flex-column text-center">
			<h1>0. Introdução</h1>
			<p>
				O jogo funciona de um jeito bem simples: caso você encontre a
				solução, basta colocar no url da página!
			</p>
			<h4>Exemplo: se a resposta for LEVEL UM</h4>
			<v-text-field
				label=".../lvl/level-um"
				variant="solo"
				color="blue"
				disabled
				append-inner-icon="mdi-magnify"
			></v-text-field>
			<v-img
				alt="Mar em movimento"
				height="17vh"
				src="https://64.media.tumblr.com/5ef9b6637f207f03394c83880355c83b/tumblr_oppipsA23V1s4u80lo1_500.gif"
			/>
		</div>
		<!-- Text -->
	</v-container>
</template>
<script setup>
// Cabeçalhos da pagina
useSeoMeta({
	title: "Introdução",
	description: "Introdução de Retrozule",
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
