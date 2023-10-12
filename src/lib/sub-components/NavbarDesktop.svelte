<script>
	import { page } from '$app/stores';
	import MafflleLogo from '$lib/MafflleLogo.svelte';
</script>

<div
	class="hidden md:flex w-full justify-between px-[3.125rem] xl:px-[7.125rem] py-[2.5rem] absolute text-white navbar z-[20]"
>
	<a href="/" class="logo flex items-center gap-[0.5rem]">
		<MafflleLogo width="20" height="20" />
		<div class="logo-text"><b>Mafflle</b> Studios</div>
	</a>
	<div class="links flex items-center gap-[1.875rem] capitalize font-normal text-[#757575]">
		<a href="/" class="link flex items-center gap-[0.625rem]">
			{#if $page.url.pathname === '/'}
				<svg
					xmlns="http://www.w3.org/2000/svg"
					width="10"
					height="10"
					viewBox="0 0 10 10"
					fill="none"
				>
					<circle cx="5" cy="5" r="5" fill="white" />
				</svg>
			{/if}
			<span class:text-white={$page.url.pathname === '/'}>Home</span>
		</a>
		<a href="/contact" class="link flex items-center gap-[0.625rem]">
			{#if $page.url.pathname === '/contact'}
				<svg
					xmlns="http://www.w3.org/2000/svg"
					width="10"
					height="10"
					viewBox="0 0 10 10"
					fill="none"
				>
					<circle cx="5" cy="5" r="5" fill="white" />
				</svg>
			{/if}
			<span class:text-white={$page.url.pathname === '/contact'}>contact us</span>
		</a>
	</div>
	<div class="social-links flex items-center gap-[1.125rem]">
		<a href="https://twitter.com/mafflle" target="_blank" class="social-link"
			><img src="/icons/Twitter.svg" alt="Twitter icon" /></a
		>
		<a href="https://www.linkedin.com/company/mafflle/" target="_blank" class="social-link"
			><img src="/icons/LinkedIn.svg" alt="LinkedIn icon" /></a
		>
	</div>
</div>

<style>
	.navbar {
		font-family: 'Manrope', sans-serif;
	}
</style>
