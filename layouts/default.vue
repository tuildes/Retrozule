<template>
	<v-app class="wrapper">
		<ClientOnly>
			<section class="d-none d-lg-flex">
				<!-- Table -->
				<div class="table" />
				<!-- Table -->
				<!-- Background CRT -->
				<v-img
					class="background"
					alt="Quarto com uma televisão antiga"
					width="100vw"
					height="90vh"
					contain
					draggable="false"
					lazy-src="/images/crt_monitor_lazy.png"
					src="/images/crt_monitor.png"
				/>
				<!-- Background CRT -->
				<!-- Page Content -->
				<div class="content">
					<div class="vhs" />
					<div class="black-border" />
					<div
						class="page-content d-flex justify-center align-center"
					>
						<NuxtPage />
					</div>
					<div class="black-border" />
				</div>
				<!-- Page Content -->
			</section>
			<section
				class="d-flex d-lg-none justify-center align-center"
				style="height: 100vh"
			>
				<Mobile />
			</section>
		</ClientOnly>
	</v-app>
</template>

<script setup lang="js">
import Mobile from "~/components/layout/Mobile.vue"
const blackBorderHeight = "3vh"
</script>
<style scoped>
@keyframes vhs-gif {
	28% {
		opacity: 0.1;
	}
	30% {
		opacity: 0.3;
	}
	33% {
		opacity: 0.2;
	}
	34% {
		opacity: 0.3;
	}
	35% {
		opacity: 0.1;
	}
}

@keyframes glitch {
	28% {
		transform: scaleX(1.005);
	}
	30% {
		transform: scaleX(1.0075);
	}
	33% {
		transform: scaleX(1.01);
	}
	34% {
		transform: scaleX(1.005);
	}
	35% {
		transform: scaleX(1.0025);
	}
}
.wrapper {
	overflow-x: hidden !important;
	width: 100vw;

	background:
		radial-gradient(
				circle,
				transparent 20%,
				#353535 20%,
				#353535 80%,
				transparent 80%,
				transparent
			)
			0% 0% / 64px 64px,
		radial-gradient(
				circle,
				transparent 20%,
				#353535 20%,
				#353535 80%,
				transparent 80%,
				transparent
			)
			32px 32px / 64px 64px,
		linear-gradient(#262626 2px, transparent 2px) 0px -1px / 32px 32px,
		linear-gradient(90deg, #262626 2px, #353535 2px) -1px 0px / 32px 32px #353535;
	background-size:
		64px 64px,
		64px 64px,
		32px 32px,
		32px 32px;
	background-color: #353535;
}

.table {
	height: 25vh;
	width: 100vw;
	position: absolute;
	z-index: 50;
	bottom: 0;
	background: rgb(32, 32, 32);
	background: linear-gradient(
		180deg,
		rgba(32, 32, 32, 1) 0%,
		rgba(85, 85, 85, 1) 2%,
		rgba(69, 69, 69, 1) 54%,
		rgba(71, 71, 71, 1) 100%
	);
}

.background {
	position: absolute;
	z-index: 50;
	pointer-events: none;
	top: 5vh;
}

.content {
	z-index: 49;
	height: 54vh;
	width: 61vh;
	top: 13.725vh;
	position: absolute;

	color: rgb(41, 41, 41);
	left: calc(50% - (23 * ((4 * 1vh) / 3)));
}

.vhs {
	background-color: #131313;
	height: 54vh;
	width: 61vh;
	left: calc(50% - (23 * ((4 * 1vh) / 3)));
	position: absolute;
	z-index: 50;
	animation: infinite vhs-gif 150ms;
	pointer-events: none;
	opacity: 0.2;
}

.page-content {
	height: calc(54vh - v-bind(blackBorderHeight) * 2);
	z-index: 45;
	animation: infinite glitch 200ms;
}

.black-border {
	height: v-bind(blackBorderHeight);
	background-color: rgb(15, 15, 15);
}
</style>
