<script lang="ts">
	import '../app.css';
	import '@fontsource-variable/roboto';
	import '@fontsource/lemon';
	import Footer from '../components/Footer/Footer.svelte';
	import Header from '../components/Header/Header.svelte';

	let { children } = $props();
</script>
<div class="container">
	<Header />
	{@render children()}
	<Footer />
</div>
