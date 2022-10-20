<script lang="ts">
import GlobalStylesProvider from '$lib/GlobalStylesProvider.svelte';

</script>

<GlobalStylesProvider>
	<div class="main-container">
		<main>
			<slot />
		</main>
		<footer>Footer</footer>
	</div>
</GlobalStylesProvider>

<style lang="scss">
	.main-container {
		position: relative;
		top: 0;
		display: flex;
		flex-direction: column;
		min-height: 100vh;
		justify-content: space-between;
	}
</style>
