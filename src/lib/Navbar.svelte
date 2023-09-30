<script>
	import DiagonalArrow from './DiagonalArrow.svelte';
	import MafflleLogo from './MafflleLogo.svelte';
</script>

<div
	class="flex w-full justify-between px-[3.125rem] xl:px-[7.125rem] py-[2.5rem] absolute text-white navbar z-[20]"
>
	<div class="logo flex items-center gap-[0.5rem]">
		<MafflleLogo width="20" height="20" />
		<div class="logo-text"><b>Mafflle</b> Studio</div>
	</div>
	<div class="links flex items-center gap-[1.875rem] capitalize font-semibold">
		<a href="/#services" class="link flex items-center gap-[0.625rem]">
			<span>Our Services</span>
			<DiagonalArrow colour="#fff" width="17" height="17" />
		</a>
		<a href="/contact" class="link flex items-center gap-[0.625rem]">
			<span>contact us</span>
			<DiagonalArrow colour="#fff" width="17" height="17" />
		</a>
	</div>
	<div class="social-links flex items-center gap-[1.125rem]">
		<a href="somesite.com" class="social-link"
			><img src="/icons/Twitter.svg" alt="Twitter icon" /></a
		>
		<a href="somesite.com" class="social-link"
			><img src="/icons/LinkedIn.svg" alt="LinkedIn icon" /></a
		>
		<a href="somesite.com" class="social-link"
			><img src="/icons/Instagram.svg" alt="Instagram icon" /></a
		>
	</div>
</div>

<style>
	.navbar {
		font-family: 'Manrope', sans-serif;
	}
</style>
