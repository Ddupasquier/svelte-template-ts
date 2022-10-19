<script lang="ts">
	import Logo from '$lib/assets/Logo.webp';
</script>

<div class="blur-border">
	<img src={Logo} alt="Svelte logo" />
</div>

<style lang="scss">
	@use 'src/styles/imports/colors.scss' as colors;

	.blur-border {
		border-radius: 50%;
		box-shadow: colors.$background inset 0 0 1rem 1rem;
	}

	img {
		width: 20rem;
		opacity: 0.2;
		border-radius: 50%;
	}
</style>
