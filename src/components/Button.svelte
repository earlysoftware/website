<script lang="ts">
	export let content: string;
	export let disabled = false;
	export let style: string;
</script>

<button on:click class={style} {disabled} aria-disabled={disabled}>{content}</button>

<style>
	button {
		border: none;
		width: 125px;
		height: 45px;

		border-radius: 5px;

		color: white;
		font-family: 'Rubik';
		font-weight: 600;
		font-size: 1.35em;
	}

	.github {
		background-color: #545e56;
	}

	.docs {
		background-color: #917c78;
	}

	button:hover {
		filter: brightness(80%);
		transition: filter 0.2s;
	}

	button:disabled {
		filter: brightness(80%);
	}
</style>
