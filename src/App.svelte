<script lang="ts">
	import { token, setGlobalTheme } from '@atlaskit/tokens';
	let bgColor = token('color.background.accent.orange.bolder', '#0065FF');
	setGlobalTheme({light: "light", dark: "legacy-dark", colorMode: 'auto'})
</script>

<main style="--bgColor: {bgColor}">
	<h1>Token</h1>
	Open the console to see the token value
	<div></div>
</main>

<style>
  	main {
		  /* Use Design Token with css variables */
		  /*background-color: var(--bgColor);*/
		  /* same as */
			background-color: var(--ds-background-accent-orange-bolder);

			/* Use Design Tokens directly */
		  color: var(--ds-text-accent-blue);
	}
</style>
