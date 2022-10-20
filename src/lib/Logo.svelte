<script lang="ts">
	import Logo from '$lib/assets/Logo.webp';
	let scroll: number
</script>

<svelte:window bind:scrollY={scroll} />

<div class="blur-border">
	<img src={Logo} alt="Svelte logo" /><br />
</div>

<style lang="scss">
	@use 'src/styles/imports/colors.scss' as colors;

	.blur-border {
		border-radius: 50%;
		// box-shadow: colors.$background inset 0 0 5rem 5rem;
		z-index: 0;
	}

	img {
		width: 15rem;
		// opacity: 0.2;
		border-radius: 50%;
	}
</style>
