<script lang="ts">
	import '../app.css';
	import Navbar from '../components/Navbar.svelte';
</script>

<svelte:head>
	<title>EarlySoftware</title>
	<meta name="description" content="Open source early access manager for the web written in Go." />
	<link rel="icon" href="src/img/favicon.ico" />
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
