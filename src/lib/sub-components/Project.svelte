<script>
	import DiagonalArrow from '$lib/DiagonalArrow.svelte';

	/**
	 * @type {string}
	 */
	export let image;
	/**
	 * @type {string}
	 */
	export let title;
	/**
	 * @type {string}
	 */
	export let about;
	/**
	 * @type  {Array<string>}
	 */
	export let tags;
	/**
	 * @type {string}
	 */
	export let link;
	/**
	 * @type {boolean}
	 */
	export let lineBreak;
</script>

<div class="w-full project md:h-[13.313rem] flex flex-col md:flex-row gap-[24px]">
	<div class="project-image w-full md:w-[40%] h-full">
		<img src={image} alt={title} class="w-full h-full" />
	</div>
	<div class="project-info w-full md:w-[70%] h-full flex flex-col justify-between">
		<div class="w-full h-full flex flex-col md:flex-row justify-between gap-[40px] md:gap-[54px]">
			<div class="w-full md:w-[80%] inner-content h-full flex flex-col justify-between gap-[40px]">
				<div class="info w-full md:h-[80%] flex flex-col gap-[20px]">
					<div class="title text-[1.25rem] font-medium">{title}</div>
					<div class="about text-[0.875rem] text-[#757575]">{about}</div>
				</div>
				<div class="tags h-[20%] flex gap-[7px]">
					{#each tags as tag}
						<div
							class="tag px-[0.75rem] py-[0.25rem] text-[#757575] border-2 border-[#757575] rounded-[20px] text-[0.625rem] md:text-[0.5rem] lg:text-[0.8rem] font-medium tracking-[2px] w-fit h-fit uppercase"
						>
							{tag}
						</div>
					{/each}
				</div>
			</div>

			<div class="w-full md:w-[20%]">
				<a
					href={link}
					class="flex items-center gap-[9px] text-[0.875rem] md:text-[0.6rem] lg:text-[1rem]"
				>
					<span class="font-medium">Visit site</span>
					<DiagonalArrow colour="#201F1F" />
				</a>
			</div>
		</div>
	</div>
</div>

{#if lineBreak}
	<hr class="py-0" />
{/if}
