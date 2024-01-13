<template>
	<v-container fluid class="wrapper IBMPlex d-flex flex-column align-center">
		<!-- Text -->
		<div class="text-content d-flex flex-column">
			<h5 v-if="!correct" class="text-center">3. Nada no jornal</h5>
			<h5 v-else class="text-center">Senha: bittersweet memories</h5>
			<v-divider class="my-2"></v-divider>
			<v-img
				alt="Jornal com vários recortes"
				src="/images/jornal-5454.png"
				height="50vh"
				class="my-2"
			/>
			<v-otp-input
				v-model="secretInput"
				theme="dark"
				:color="stateInput"
				:loading="stateLoading"
				:disabled="correct"
				width="50%"
				length="4"
			/>
			<div class="d-flex justify-center mt-2">
				<v-btn
					width="50%"
					variant="outlined"
					:disabled="correct"
					@click="verifier"
				>
					Enviar
				</v-btn>
			</div>
		</div>
		<!-- Text -->
	</v-container>
</template>
<script setup>
const secretInput = ref("----")
const stateInput = ref("white")
const stateLoading = ref(false)
const correct = ref(false)

function verifier() {
	stateLoading.value = true
	stateInput.value = "white"
	setTimeout(() => {
		stateLoading.value = false
		if (secretInput.value == "7834") {
			correct.value = true
			stateInput.value = "success"
		} else {
			stateInput.value = "error"
		}
	}, 2000)
}

// Cabeçalhos da pagina
useSeoMeta({
	title: "Fase 03",
	description: "Fase 03 de Retrolure",
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
