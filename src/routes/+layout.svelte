<script lang="ts">
	import AboveFold from '$lib/AboveFold.svelte';
	import GlobalStylesProvider from '$lib/GlobalStylesProvider.svelte';
	import Bottom3 from '$lib/Waves/BottomWave.svelte';
	import Top3 from '$lib/Waves/TopWave.svelte';
	import WholeWave from '$lib/WholeWave.svelte';
</script>

<GlobalStylesProvider>
	<div class="main-container">
		<AboveFold />
		<Top3 />
		<!-- <WholeWave /> -->
		<main>
			<slot />
		</main>
		<Bottom3 />
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
