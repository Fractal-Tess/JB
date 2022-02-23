<script lang="ts">
	export let onClick: () => void = () => {};
	export let text: string;
	export let textSize: 1 | 2 | 3 | 4 | 5 | 6 | 7 = 3;
</script>

<div>
	<button on:click={onClick}>{text}</button>
</div>

<style lang="scss">
	div,
	button {
		@apply h-full w-full;
		button {
			@apply shadow-lg shadow-neutral-500/50 rounded-3xl border-2 border-neutral-400 font-bold text-neutral-500;
		}
	}
</style>
