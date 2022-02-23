<script lang="ts">
	export let icon = '';
	export let size = 6;
	export let onClick: () => void = () => {};
	let iconSize;
	$: {
		switch (size) {
			case 1:
				iconSize = ' text-xl';
				break;
			case 2:
				iconSize = ' text-2xl';
				break;
			case 3:
				iconSize = ' text-4xl';
				break;
			case 4:
				iconSize = ' text-5xl';
				break;
			case 5:
				iconSize = ' text-7xl';
				break;
			case 6:
				iconSize = ' text-9xl';
				break;
		}
	}
</script>

<div>
	<i class={icon + iconSize} on:click={onClick} />
</div>

<style lang="scss">
	i {
		cursor: pointer;
		padding: 0.5rem;
	}
</style>
