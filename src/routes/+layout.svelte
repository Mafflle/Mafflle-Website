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
