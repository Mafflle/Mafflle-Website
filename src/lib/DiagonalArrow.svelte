<script>
	/**
	 * Colour of the diagonal arrow
	 * @type string
	 */
	export let colour = 'white';
	/**
	 * Arrow Width
	 *
	 * @type       string
	 */
	export let width = '14';
	/**
	 * Arrow Height
	 *
	 * @type       string
	 */
	export let height = '14';
</script>

<svg {width} {height} viewBox="0 0 14 14" fill="none" xmlns="http://www.w3.org/2000/svg">
	<path
		d="M3.5 11.0833L11.0833 3.5M11.0833 3.5V10.78M11.0833 3.5H3.80333"
		stroke={colour}
		stroke-linecap="round"
		stroke-linejoin="round"
	/>
</svg>
