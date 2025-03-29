<script lang="ts">
	import '../app.css';
	import '@fontsource-variable/roboto';
	import '@fontsource/lemon';
	import Footer from '../components/Footer/Footer.svelte';
	import Header from '../components/Header/Header.svelte';
	import Hero from '../components/Main/others/Hero.svelte';

	let { children } = $props();
</script>
<div class="container overflow-hidden">
	<Header />
	<Hero />
	{@render children()}
	<Footer />
</div>
