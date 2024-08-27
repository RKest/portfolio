<script lang="ts">
	export let title: string;
	export let description: string;
	export let href: string;
	export let video: string;

	export let rowspan: number = 1;
</script>

<div class="m-8" style="grid-row: span {rowspan} / auto">
	<video controls>
		<source src={video} />
		<track kind="captions" />
	</video>
	<a
		class="text-blue-600 dark:text-blue-500 hover:underline cursor-pointer text-xl mt-1 block"
		{href}
		target="_blank"
	>
		{title}
	</a>
	<p>{@html description}</p>
</div>

<style>
	video {
		max-height: 80vh;
		width: auto;
	}
</style>
