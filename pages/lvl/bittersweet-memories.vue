<template>
	<v-container fluid class="wrapper IBMPlex d-flex flex-column align-center">
		<!-- Text -->
		<div class="text-content d-flex flex-column">
			<h5 class="text-center">4. bittersweet memories</h5>
			<v-divider class="my-2"></v-divider>
			<section class="d-flex flex-column">
				<v-btn variant="text" @click="openDialog(`e`)">
					Oldschool (Ft. Biffe)
				</v-btn>
				<v-btn variant="text" @click="openDialog(`c`)">
					The Story
				</v-btn>
				<v-btn variant="text" @click="openDialog(`D`)">
					Melhor Não (Ft. Aki Punou)
				</v-btn>
				<v-btn variant="text" @click="openDialog(`D`)"> Saúde </v-btn>
				<v-btn variant="text" @click="openDialog(`i`)">
					O Filho Pródigo
				</v-btn>
				<v-btn variant="text" @click="openDialog(`i`)">
					Máquina do Tempo
				</v-btn>
				<v-btn variant="text" @click="openDialog(`V`)">
					Dirty Dancing
				</v-btn>
				<v-btn variant="text" @click="openDialog(`s`)">
					Let it Pour
				</v-btn>
				<v-btn variant="text" @click="openDialog(`o`)">
					Back Home (Ft. Massaru)
				</v-btn>
				<v-btn variant="text" @click="openDialog(`n`)">
					Quase Perfeito
				</v-btn>
				<v-btn variant="text" @click="openDialog(`i`)">
					Prefiro Morrer (Ft. D$ Luqi)
				</v-btn>
				<v-btn variant="text" @click="openDialog(`l`)">
					Flores de Outro Carnaval
				</v-btn>
			</section>
		</div>
		<!-- Text -->
	</v-container>
</template>
<script setup>
function openDialog(char) {
	window.alert(`${char}`)
}
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
