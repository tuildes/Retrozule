<template>
	<v-container fluid class="wrapper IBMPlex d-flex flex-column align-center">
		<!-- Text -->
		<div class="text-content d-flex flex-column text-center">
			<h5 class="text-center">Fim!</h5>
			<v-divider class="my-2"></v-divider>
			<v-img
				alt="Personagens de anime dando parabéns"
				height="17vh"
				class="mt-3"
				src="https://gifdb.com/images/high/congratulations-anime-characters-pwsk91uegcty6tx6.webp"
			/>
			<h2>Parabéns!</h2>
			<p>
				Esse é um jogo bem curtinho de puzzles, espero que tenha se
				divertido :)
			</p>
			<p>
				Talvez algum dia eu faça uma versão mais completa, mas por
				enquanto este é o <b>fim</b>.
			</p>
		</div>
		<!-- Text -->
	</v-container>
</template>
<script setup>
// Cabeçalhos da pagina
useSeoMeta({
	title: "FIM!",
	description: "Final do Retrolure",
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
	background: url(https://www.gifstop.com/images/backgrounds/bluewave.gif)
		100% 100% no-repeat;
}

.text-content {
	overflow-y: auto;
	width: 95%;
	gap: 10px;
}
</style>
