<template>
	<v-container fluid class="wrapper IBMPlex d-flex flex-column align-center">
		<!-- Text -->
		<div class="text-content d-flex flex-column text-center">
			<h5>1. Level 1</h5>
			<v-divider class="my-2"></v-divider>
			<span>Entendeu o jogo? Então, boa sorte :)</span>
			<v-img
				alt="Menina folheando uma revista"
				src="https://64.media.tumblr.com/2b1a727e2a3e5f3bc8628c5328fbcd5b/tumblr_ppq2feUMPf1x6a7yto1_500.gif"
				height="20vh"
				class="my-2"
			/>
			<p>&nbsp;</p>
			<p>&nbsp;</p>
			<p>&nbsp;</p>
			<p>&nbsp;</p>
			<p>&nbsp;</p>
			<p>&nbsp;</p>
			<p>&nbsp;</p>
			<p>&nbsp;</p>
			<p>&nbsp;</p>
			<p>&nbsp;</p>
			<p>&nbsp;</p>
			<p>&nbsp;</p>
			<p>&nbsp;</p>
			<p>&nbsp;</p>
			<p>&nbsp;</p>
			<p>lembrancas-de-outono</p>
			<p>&nbsp;</p>
			<p>&nbsp;</p>
			<p>&nbsp;</p>
			<p>&nbsp;</p>
			<p>&nbsp;</p>
			<p>&nbsp;</p>
			<p>&nbsp;</p>
			<p>&nbsp;</p>
			<p>&nbsp;</p>
			<p>&nbsp;</p>
		</div>
		<!-- Text -->
	</v-container>
</template>
<script setup>
// Cabeçalhos da pagina
useSeoMeta({
	title: "Fase 01",
	description: "Fase 01 de Retrozule",
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
	background: rgb(46, 38, 75);
}

.text-content {
	overflow-y: auto;
	width: 95%;
}

p {
	color: rgb(46, 38, 75);
}
</style>
