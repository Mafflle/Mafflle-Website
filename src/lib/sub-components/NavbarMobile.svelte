<script>
	import MafflleLogo from '$lib/MafflleLogo.svelte';
</script>

<div
	class="navbar flex justify-between items-center md:hidden w-full px-[1.25rem] py-[2.5rem] absolute h-[3rem] z-[20] navbar text-white"
>
	<a href="/" class="logo flex items-center gap-[0.5rem]">
		<MafflleLogo width="20" height="20" />
		<div class="logo-text"><b>Mafflle</b> Studios</div>
	</a>
	<div class="menu">
		<svg xmlns="http://www.w3.org/2000/svg" width="24" height="9" viewBox="0 0 24 9" fill="none">
			<line x1="0.325684" y1="8.5" x2="24.0001" y2="8.5" stroke="white" />
			<line y1="0.5" x2="23.6744" y2="0.5" stroke="white" />
		</svg>
	</div>
</div>

<style>
	.navbar {
		font-family: 'Manrope', sans-serif;
	}
</style>
