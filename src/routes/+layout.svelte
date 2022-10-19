<script lang="ts">
	import AboveFold from '$lib/AboveFold.svelte';
	import GlobalStylesProvider from '$lib/GlobalStylesProvider.svelte';
	import FrontWaves from '$lib/Waves/FrontWaves.svelte';
	import BackWaves from '$lib/Waves/BackWaves.svelte';
	import WholeWave from '$lib/WholeWave.svelte';
</script>

<GlobalStylesProvider>
	<div class="main-container">
		<AboveFold />
		<BackWaves />
		<!-- <WholeWave /> -->
		<main>
			<slot />
		</main>
		<FrontWaves />
		<footer>Footer</footer>
	</div>
</GlobalStylesProvider>

<style lang="scss">
	.main-container {
		display: grid;
		grid-template-rows: 1fr auto;
		height: 100vh;
	}
</style>
