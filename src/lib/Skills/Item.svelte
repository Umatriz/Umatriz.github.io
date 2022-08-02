<script lang="ts">
	export let name: string;
	export let learning: boolean = false;
</script>

<div class="Item">
	<div class="Icon"><slot /></div>
	{#if learning === true}
		<span class="Text Learning">{name}</span>
	{:else}
		<span class="Text">{name}</span>
	{/if}
	{#if learning === true}
		<span class="HelpText">Learning</span>
	{/if}
</div>

<style>
	.Item {
		display: flex;
		align-items: center;
		justify-content: center;
		gap: 0.3rem;
	}
	.Icon {
		height: 2rem;
		width: 2rem;
	}
	.Text {
		font-size: 1.3rem;
	}
	.Learning {
		color: #7b7b7b;
	}
	.HelpText {
		position: relative;
		width: auto;
		color: #000;
		font-size: 14px;
		transition: 0.3s ease-in-out;
		margin-left: 30px;
		opacity: 0;
		visibility: hidden;
		text-align: center;
	}
	.HelpText::before {
		content: '';
		position: absolute;
		transition: 0.3s ease-in-out;
		top: 0;
		right: -0.8rem;
		width: 2px;
		height: 0;
		background-color: #1a132f;
		border-radius: 2px;
	}
	.Item:hover .HelpText {
		opacity: 1;
		visibility: visible;
		transform: translateX(-20px);
	}
	.Item:hover .HelpText::before {
		height: 100%;
	}
</style>
