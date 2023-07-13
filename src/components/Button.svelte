<script lang="ts">
	export let content: string;
	export let disabled = false;
</script>

<div id="button-wrapper">
	<button on:click {disabled} aria-disabled={disabled}>{content}</button>
</div>

<style>
	button {
		border: none;
		width: 125px;
		height: 45px;

		border-radius: 5px;

		background-color: #393939;
		color: white;
		font-family: 'Inter';
		font-weight: 700;
	}

	button:disabled {
		filter: brightness(80%);
	}
</style>
