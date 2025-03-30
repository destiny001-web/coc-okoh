<script lang="ts">
	import '../app.css';
	import '@fontsource-variable/roboto';
	import '@fontsource/lemon';
	import Footer from '../components/Footer/Footer.svelte';
	import Header from '../components/Header/Header.svelte';
	import Hero from '../components/Main/others/Hero.svelte';

	let { children } = $props();
</script>
<div class="container overflow-hidden text-sm">
	<div>
		<section class="relative w-full pt-2 pb-10 text-white md:py-5 md:pb-10 xl:h-100 2xl:h-200">
			<div class="absolute inset-0 bg-cover bg-center w-full" style="background-image: url('/hero/hero.jpg');"></div>
			<div class="absolute inset-0 bg-black opacity-50"></div>
			<div class="relative z-10 gap-5">
				<div>
					<Header />
					<Hero />
				</div>		
			</div>
		</section>
		{@render children()}
		<Footer />
	</div>
</div>
