<script>
	import favicon from '$lib/favicon.ico';
	import '$lib/styles.css'

	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
	<title>Solar Engine</title>
</svelte:head>

{@render children()}
