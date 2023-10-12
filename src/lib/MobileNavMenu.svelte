<script>
	import { page } from '$app/stores';
	import LinkedIn from './icons/LinkedIn.svelte';
	import Twitter from './icons/Twitter.svelte';
	import { navOpen } from './store';
	const closeNav = () => {
		navOpen.set(false);
	};
</script>

{#if $navOpen}
	<div
		class="h-screen w-screen z-50 backdrop-blur-lg fixed flex md:hidden flex-col justify-center items-center gap-[6rem]"
	>
		<div class="absolute top-8 right-5">
			<button on:click={closeNav}>
				<img src="/icons/Close.svg" alt="close button" />
			</button>
		</div>
		<div
			class="flex flex-col gap-[2.5rem] items-center justify-center text-[2.5rem] text-[#D9D9D9] font-[500]"
		>
			<a href="/" class="link flex items-center gap-[0.625rem]">
				{#if $page.url.pathname === '/'}
					<svg
						xmlns="http://www.w3.org/2000/svg"
						width="21"
						height="20"
						viewBox="0 0 21 20"
						fill="none"
					>
						<circle cx="10.5" cy="10" r="10" fill="white" />
					</svg>
				{/if}
				<span class:text-white={$page.url.pathname === '/'}>Home</span>
			</a>
			<a href="/contact" class="link flex items-center gap-[0.625rem]">
				{#if $page.url.pathname === '/contact'}
					<svg
						xmlns="http://www.w3.org/2000/svg"
						width="21"
						height="20"
						viewBox="0 0 21 20"
						fill="none"
					>
						<circle cx="10.5" cy="10" r="10" fill="white" />
					</svg>
				{/if}
				<span class:text-white={$page.url.pathname === '/contact'}>Contact</span>
			</a>
		</div>
		<div class="icons flex gap-4">
			<a href="https://twitter.com/mafflle" target="_blank">
				<Twitter width={30} height={30} />
			</a>
			<a href="https://www.linkedin.com/company/mafflle/" target="_blank">
				<LinkedIn width={30} height={30} />
			</a>
		</div>
	</div>
{/if}
