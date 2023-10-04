<script>
	import HeroElements from './sub-components/HeroElements.svelte';
	import HeroVector from './sub-components/HeroVector.svelte';
</script>

<div class="overflow-hidden h-[77vh] lg:h-[91vh]">
	<HeroVector />

	<div
		class="h-full h-[77vh] lg:h-[98vh] xl:w-screen hero text-white flex items-center px-[1rem] lg:px-[3.125rem] xl:px-[12.125rem] z-[9] relative"
	>
		<HeroElements />
	</div>
</div>
