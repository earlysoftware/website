<script>
	import { goto } from '$app/navigation';
	import Button from '../components/Button.svelte';
</script>

<svelte:head>
	<title>EarlySoftware</title>
</svelte:head>

<div>
	<span id="h1-background">
		<h1>EarlySoftware</h1>
	</span>

	<span id="text-button-wrapper">
		<p>
			Open source <span id="poppins-800">early access manager</span> for the web <br /> written in
			<span id="go-text">Go</span>.
		</p>

		<span id="button">
			<span id="github">
				<Button
					style="github"
					content="GitHub"
					on:click={() => goto('https://github.com/earlysoftware/core')}
				/>
			</span>

			<span id="documentation">
				<Button style="docs" content="Docs" />
			</span>
		</span>
	</span>
</div>

<style>
	:root {
		--background-color: #e7ebe5;
	}

	:global(body) {
		background-color: var(--background-color);
	}

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

	p {
		margin-top: 15px;
	}

	#button {
		position: relative;
		top: 30px;
	}

	#h1-background {
		background-color: rgba(102, 119, 97, 0.42);
		border-radius: 24px;

		padding: 5px 10px;

		position: relative;
		right: 100px;
	}

	p {
		font-family: 'Lora';
		font-weight: 700;
		font-size: 1.4em;
	}

	#poppins-800 {
		font-weight: 800;
		font-style: italic;
		font-family: 'Poppins';

		line-height: 30px;
	}

	#go-text {
		color: #545e56;

		font-weight: 900;
	}

	#go-text::selection {
		color: black;
	}

	h1 {
		font-family: 'Rubik';
		font-weight: 800;

		font-size: clamp(2.3em, 10vw, 3.5em);
		word-break: break-all;
	}

	@media (max-width: 767px) {
		#h1-background {
			right: 0px;
			border-radius: 15px;
		}

		p {
			text-align: center;
		}

		#text-button-wrapper {
			display: block;
		}

		#button {
			display: flex;
			justify-content: center;
			gap: 5px;
		}
	}
</style>
