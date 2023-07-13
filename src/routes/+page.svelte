<script>
	import { goto } from '$app/navigation';
	import Button from '../components/Button.svelte';
</script>

<svelte:head>
	<title>EarlySoftware</title>
</svelte:head>

<div>
	<h1>EarlySoftware</h1>
	<p>Early access manager for the web.</p>

	<span id="button">
		<span id="github">
			<Button content="GitHub" on:click={() => goto('https://github.com/earlysoftware/core')} />
		</span>

		<span id="documentation">
			<Button content="Documentation" />
		</span>
	</span>
</div>

<style>
	div {
		height: 100%;
		width: 100%;

		position: fixed;

		display: flex;
		align-items: center;
		justify-content: center;
		flex-direction: column;
	}

	#github,
	#documentation {
		display: inline-block;
	}

	p,
	#button {
		margin-top: 15px;
	}

	h1 {
		font-size: 3em;
		font-weight: 800;
	}
</style>
