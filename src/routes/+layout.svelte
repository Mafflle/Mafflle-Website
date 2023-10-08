<script>
	import MobileNavMenu from '$lib/MobileNavMenu.svelte';
	import '../app.css';
</script>

<MobileNavMenu />

<slot />
<svelte:head>
	<link rel="preconnect" href="https://fonts.googleapis.com" />
	<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
	<link href="https://fonts.googleapis.com/css2?family=Manrope&display=swap" rel="stylesheet" />
</svelte:head>
