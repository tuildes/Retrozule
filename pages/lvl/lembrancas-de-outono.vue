<template>
	<v-container fluid class="wrapper IBMPlex d-flex flex-column align-center">
		<!-- Text -->
		<div class="text-content d-flex flex-column">
			<h5 class="text-center">2. Lembranças de outono</h5>
			<v-divider class="my-2"></v-divider>
			<p>...</p>
			<p>Vagando por vagões de divagação</p>
			<p>Devagar, estação por estação passa por mim</p>
			<p>Túneis e clarões, grandes vegetações</p>
			<p>Poucas habitações até chegar ao fim da jornada</p>
			<p>&nbsp;</p>
			<p>Então leio lembranças do meu diário mental</p>
			<p>Vejo humanos amenos e demônios entre os neurônios</p>
			<p>Onde a memória mora por muitos anos</p>
			<p>O vapor vai por nuvens no céu</p>
			<p>...</p>
			<h5 class="my-2">Estações - Makalister & Matéria Prima</h5>
			<v-img
				alt="Rádio"
				src="https://images-wixmp-ed30a86b8c4ca887773594c2.wixmp.com/f/3b537a2a-9e9a-47c9-b103-26dc4cc96e81/dg8b3in-fa99fe3f-24d7-4117-9332-365b5103034d.gif?token=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJ1cm46YXBwOjdlMGQxODg5ODIyNjQzNzNhNWYwZDQxNWVhMGQyNmUwIiwiaXNzIjoidXJuOmFwcDo3ZTBkMTg4OTgyMjY0MzczYTVmMGQ0MTVlYTBkMjZlMCIsIm9iaiI6W1t7InBhdGgiOiJcL2ZcLzNiNTM3YTJhLTllOWEtNDdjOS1iMTAzLTI2ZGM0Y2M5NmU4MVwvZGc4YjNpbi1mYTk5ZmUzZi0yNGQ3LTQxMTctOTMzMi0zNjViNTEwMzAzNGQuZ2lmIn1dXSwiYXVkIjpbInVybjpzZXJ2aWNlOmZpbGUuZG93bmxvYWQiXX0.M7xZY-ZNifVMmHjgwS5hBWN8DRW0CgAd_UAgrsSKzco"
				height="15vh"
				class="my-2"
			/>
		</div>
		<!-- Text -->
	</v-container>
</template>
<script setup>
// Cabeçalhos da pagina
useSeoMeta({
	title: "Fase 02",
	description: "Fase 02 de Retrolure",
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
	color: rgb(255, 255, 255);
	background: rgb(52, 11, 59);
}

.text-content {
	overflow-y: auto;
	width: 95%;
}
</style>
