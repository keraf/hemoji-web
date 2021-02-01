<script lang="ts">
	import hemoji from 'hemoji';
	import Playground from './components/Playground.svelte';
	import Usage from './components/Usage.svelte';
	import Info from './components/Info.svelte';
	import Header from './components/Header.svelte';
	import Footer from './components/Footer.svelte';
	
	let input: string = 'Welcome!';
	let length: number = 6;
	$: result = hemoji(input, { length });
</script>

<main>
	<Header />	
	<Playground bind:input={input} bind:length={length} result={result} />
	<Info />
	<Usage input={input} length={length} result={result} />
	<Footer />
</main>

<style>
	main {
		padding: 1em;

		display: flex;
		flex-direction: column;
		align-items: center;
	}
</style>