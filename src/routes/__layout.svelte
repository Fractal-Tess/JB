<script>
	import '../app.scss';
	import Header from '$lib/components/Header.svelte';
	import { theme } from '$lib/components/stores/theme';
</script>

<main class="dark">
	<Header />
	<content><slot /></content>
	<footer />
</main>

<style>
	main {
		@apply flex flex-col border-4 border-red-300 min-h-screen;
	}
</style>
