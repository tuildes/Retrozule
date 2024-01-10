<template>
	<v-container fluid class="wrapper IBMPlex d-flex flex-column align-center">
		<!-- Text -->
		<div class="text-content d-flex flex-column">
			<h5 class="text-center">2. Nada no jornal</h5>
			<v-divider class="my-2"></v-divider>
			<v-img
				alt="Folheando um caderno em japonês"
				src="https://i.pinimg.com/originals/3b/13/8c/3b138cfbb52c29b1aab2f55fbdd7f473.gif"
				height="15vh"
				class="my-2"
			/>
			<v-otp-input v-model="secretInput" length="4" />
			{{ secretInput }}
		</div>
		<!-- Text -->
	</v-container>
</template>
<script setup>
const secretInput = ref("0000")
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
	background: rgb(36, 36, 36);
}

.text-content {
	overflow-y: auto;
	width: 95%;
}
</style>
