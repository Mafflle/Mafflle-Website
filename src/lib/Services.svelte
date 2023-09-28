<script>
	let services = [
		{
			number: '01',
			name: 'Software development'
		},
		{
			number: '02',
			name: 'UI/UX design'
		},
		{
			number: '03',
			name: 'Brand identity design'
		}
	];
</script>

<div class="xl:px-[12.125rem] px-[2.5rem] py-[3.063rem] bg-[#06050A] text-white" id="services">
	<h3 class="services-header text-[0.75rem] tracking-[2.4px]">SERVICES</h3>
	<div class="services-list pt-[5.625rem]">
		{#each services as service}
			<div
				class="service flex justify-between pb-[10px] py-[3.125rem] border-b border-b-white items-center"
			>
				<div class="service-number text-[0.75rem] tracking-[2.4px]">{service.number}</div>
				<div class="service-name text-[3rem]">{service.name}</div>
			</div>
		{/each}
	</div>
</div>
