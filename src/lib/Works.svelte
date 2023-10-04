<script>
	import Project from './sub-components/Project.svelte';

	const projects = [
		{
			image: '/img/uruggo.png',
			title: 'Uruggo',
			about:
				'Uruggo is a real estate platform designed to simplify apartment hunting and redefine the housing experience in Nigeria and Benin Republic. With a commitment to user-centric design, Uruggo empowers both real estate agents and renters by providing a comprehensive platform for property listings and searches.',
			link: 'https://uruggo.com',
			tags: ['UI/UX DESIGN', 'Web Development'],
			lineBreak: true
		},
		{
			image: '/img/sisi-oni-dukia.png',
			title: 'Sisi oni dukia',
			about:
				'Sisi Oni Dukia is a real estate platform revolutionizing apartment hunting and the housing experience in Nigeria . With a focus on user-centric design, it empowers real estate agents and renters through a comprehensive property listing and search platform',
			link: 'https://uruggo.com',
			tags: ['Web Development'],
			lineBreak: false
		}
	];
</script>

<div class="xl:px-[12.125rem] px-[2.5rem] min-h-screen sm:py-[5.625rem]">
	<h2 class="header text-[1.875rem] md:text-[3rem] font-semibold">Featured works</h2>
	<div class="projects py-10 flex flex-col gap-[6.25rem]">
		{#each projects as project}
			<Project
				image={project.image}
				title={project.title}
				about={project.about}
				tags={project.tags}
				link={project.link}
				lineBreak={project.lineBreak}
			/>
		{/each}
	</div>
</div>
