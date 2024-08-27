<script lang="ts">
	import Card from "$lib/card.svelte";
</script>

<h1 class="mt-8 text-4xl font-bold w-full text-center">
	Familiar technologies
</h1>
<img src="skills.svg" alt="Technologies" class="mx-auto" />
<hr class="w-1/3 mx-auto my-8" />
<h1 class="text-4xl font-bold w-full text-center">Project demos</h1>
<main class="grid justify-center">
	<Card
		title="Skillscatter"
		description="A tool for visualizing skills written in Svelte for UX with C++ compiled to WASM for generating the word cloud."
		video="skillscatter.webm"
		href="https://rkest.github.io/skillscatter/"
	/>
	<Card
		title="Music visualizer"
		description="Music visualizer written for STM32 and MEMS analog microphone implemented using FFT. 
		<br>Make sure to turn up the sound on this one."
		video="fourier.mp4"
		rowspan={2}
		href="https://github.com/RKest/fourier_stm"
	/>
	<Card
		title="LSTree"
		description="Procedurally generated trees using Lyndenmayer systems rendered with OpenGL."
		video="lsystems.mp4"
		href="https://github.com/RKest/LSTree"
	/>
	<Card
		title="Mahai"
		description="Reinforcement network playing Riichi Mahjong implemented based on stable baselines3 implementation."
		video="mahjong.webm"
		href="https://github.com/RKest/mahaipp"
	/>
</main>

<hr class="w-1/3 mx-auto my-8" />

<h1 class="mt-8 text-4xl font-bold w-full text-center">Contact</h1>
<p class="text-center">
	<a href="mailto:max.ind@o2.pl">max.ind@o2.pl</a>
	<br />
	<span>+48 660 811 115</span>
</p>
<hr class="w-1/3 mx-auto my-8" />

<style>
	img {
		width: max(33%, 300px);
	}

	:global(body) {
		font-family: IBMPlexMono, monospace;
	}
	.grid {
		justify-content: center;
		grid-template-columns: 2fr 1fr;
	}
	@media (max-width: 768px) {
		.grid {
			grid-template-columns: 1fr;
		}
	}
</style>
