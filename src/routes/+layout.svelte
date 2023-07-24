<script lang="ts">
	import '../app.css';
	import Navbar from '../components/Navbar.svelte';
	import logo from '$lib/assets/favicon.ico';
</script>

<svelte:head>
	<title>EarlySoftware</title>
	<meta name="description" content="Open source early access manager for the web written in Go." />
	<link rel="icon" href={logo} />
</svelte:head>

<Navbar />

<slot />

<style>
	:root {
		--background-color: #e7ebe5;
	}

	:global(body) {
		background-color: var(--background-color);
	}
</style>
