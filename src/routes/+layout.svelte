<script>
	import MobileNavMenu from '$lib/MobileNavMenu.svelte';
	import { onMount } from 'svelte';
	import '../app.css';
	// import Lenis from '@studio-freight/lenis';

	// onMount(() => {
	// 	const lenis = new Lenis();

	// 	/**
	// 	 * @param {number} time
	// 	 */
	// 	function raf(time) {
	// 		lenis.raf(time);
	// 		requestAnimationFrame(raf);
	// 	}

	// 	requestAnimationFrame(raf);
	// });
</script>

<MobileNavMenu />

<slot />
<svelte:head>
	<link rel="preconnect" href="https://fonts.googleapis.com" />
	<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
	<link href="https://fonts.googleapis.com/css2?family=Manrope&display=swap" rel="stylesheet" />

	<!-- HTML Meta Tags -->
	<title>Mafflle</title>
	<meta name="description" content="undefined" />

	<!-- Facebook Meta Tags -->
	<meta property="og:url" content="https://maffle-website.vercel.app" />
	<meta property="og:type" content="website" />
	<meta property="og:title" content="Mafflle" />
	<meta
		property="og:description"
		content="Mafflle studios help businesses and brands across industries build a better digital identity"
	/>
	<meta property="og:image" content="https://maffle-website.vercel.app/img/intro-image.png" />

	<!-- Twitter Meta Tags -->
	<meta name="twitter:card" content="summary_large_image" />
	<meta property="twitter:domain" content="maffle-website.vercel.app" />
	<meta property="twitter:url" content="https://maffle-website.vercel.app" />
	<meta name="twitter:title" content="Mafflle" />
	<meta
		name="twitter:description"
		content="Mafflle studios help businesses and brands across industries build a better digital identity"
	/>
	<meta name="twitter:image" content="https://maffle-website.vercel.app/img/intro-image.png" />
</svelte:head>

<style>
	@keyframes -global-fade-in-bottom {
		0% {
			-webkit-transform: translateY(50px);
			transform: translateY(50px);
			opacity: 0;
		}
		100% {
			-webkit-transform: translateY(0);
			transform: translateY(0);
			opacity: 1;
		}
	}
</style>
