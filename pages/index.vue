<template>
	<v-container fluid class="disco-wrapper ma-0 pa-0"> texto </v-container>
</template>
<script setup>
// Cabeçalhos da pagina
useSeoMeta({
	title: "Index",
	description: "Descricao index",
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
<style scoped></style>
