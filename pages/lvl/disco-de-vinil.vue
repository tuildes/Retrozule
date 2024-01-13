<template>
	<v-container fluid class="wrapper IBMPlex d-flex flex-column align-center">
		<!-- Text -->
		<div class="text-content d-flex flex-column">
			<h5 class="text-center">5. Disco de Vinil</h5>
			<v-divider class="my-2"></v-divider>
			<v-img
				alt="Disco de vinil girando"
				height="17vh"
				class="mt-3"
				src="https://i.pinimg.com/originals/b5/39/39/b539391edeaed377d62a3be4fc879c8b.gif"
			/>
			<section class="d-flex flex-column align-center">
				<v-btn
					prepend-icon="mdi-play"
					variant="plain"
					width="50%"
					class="mt-6"
					@click="changeMusic()"
				>
					Trocar de música
				</v-btn>
				<span class="mt-2">
					Tocando agora: <b>{{ music }}</b>
				</span>
				<v-progress-linear
					model-value="20"
					color="blue"
					stream
					class="mt-4"
				/>
				<audio v-if="morse" controls class="mt-4">
					<source src="/morse.wav" type="audio/wav" />
					Seu navegador não suporta o elemento de audio
				</audio>
			</section>
		</div>
		<!-- Text -->
	</v-container>
</template>
<script setup>
const numChanges = ref(0)
const musicList = [
	"God`s Plan - Drake",
	"The Lord And Me - Yung Li",
	"Desabafos Não Mentem - Rodrigo Zin",
	"GANG GANG - JACKBOYS",
	"Scared Of The Dark - Lil Wayne",
	"Futón - Makalister, Beli Remour",
	"Sonhar - Yung Li",
	"Mona Lisa - Dominic Fike",
	"rockstar - Post Malone",
	"Carta de um Anjo - Menestrel",
]
const morse = ref(false)
const music = ref("me encontra lá :) - Gab Ferreira")

function changeMusic() {
	numChanges.value++
	if (numChanges.value > 18) {
		morse.value = true
		music.value = "??? - ???"
	} else {
		music.value = musicList[Math.floor(Math.random() * musicList.length)]
	}
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
	background: rgb(11, 28, 52);
}

.text-content {
	overflow-y: auto;
	width: 95%;
}
</style>
