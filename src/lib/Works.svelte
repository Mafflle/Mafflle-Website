<script>
	import Project from './sub-components/Project.svelte';

	const projects = [
		{
			image: '/img/placeholder.png',
			title: 'Uruggo',
			about:
				'From highly skilled software engineers to exceptionally talented designers, Maffle brings together a fusion of top-tier talent in the digital arena. Our team is a harmonious blend of',
			link: 'https://uruggo.com',
			tags: ['UI/UX DESIGN', 'Web Development']
		},
		{
			image: '/img/placeholder.png',
			title: 'Sisi oni dukia',
			about:
				'From highly skilled software engineers to exceptionally talented designers, Maffle brings together a fusion of top-tier talent in the digital arena. Our team is a harmonious blend of',
			link: 'https://uruggo.com',
			tags: ['Web Development']
		},
		{
			image: '/img/placeholder.png',
			title: 'Sisi oni dukia',
			about:
				'From highly skilled software engineers to exceptionally talented designers, Maffle brings together a fusion of top-tier talent in the digital arena. Our team is a harmonious blend of',
			link: 'https://uruggo.com',
			tags: ['Web Development']
		}
	];
</script>

<div class="xl:px-[12.125rem] px-[2.5rem]">
	<h2 class="header text-[3rem] font-semibold">Featured works</h2>
	<div class="projects py-10 flex flex-col gap-[6.25rem]">
		{#each projects as project}
			<Project
				image={project.image}
				title={project.title}
				about={project.about}
				tags={project.tags}
				link={project.link}
			/>
		{/each}
	</div>
</div>
