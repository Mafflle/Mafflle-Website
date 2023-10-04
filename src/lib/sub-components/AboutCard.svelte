<script>
	import DiagonalArrow from '$lib/DiagonalArrow.svelte';
	/**
	 * Title of the about card
	 * @type string
	 */
	export let title;
	/**
	 * Content in the about card
	 * @type string
	 */
	export let content;
</script>

<div
	class="about-card w-full md:w-1/2 bg-[#F3F3F3] text-[#201F1F] h-[12.938rem] md:h-[15.5rem] lg:h-[13.063rem] rounded-lg backdrop-filter-[blur(100px)] flex flex-col justify-around px-[1.5rem] py-[1.25rem] gap-[1.188rem]"
>
	<div
		class="card-title flex justify-between gap-[0.625rem] font-bold text-[1rem] md:text-[1.4rem]"
	>
		<span>{title}</span>
		<DiagonalArrow colour="#201F1F" />
	</div>
	<div class="card-content text-[0.80rem] text-[#757575] text-[0.75rem]">
		{content}
	</div>
</div>
