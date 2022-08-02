<script>
	import Python from '$lib/Icons/Python.svelte';
	import Js from '$lib/Icons/Js.svelte';
	import Django from '$lib/Icons/Django.svelte';
	import Svelte from '$lib/Icons/Svelte.svelte';
	import Git from '$lib/Icons/Git.svelte';
	import Md from '$lib/Icons/Md.svelte';
	import Nest from '$lib/Icons/Nest.svelte';
	import Ts from '$lib/Icons/Ts.svelte';
	import Item from './Item.svelte';
</script>

<section class="Skills" id="skills">
	<div class="List">
		<div class="Group">
			<span class="Title">Programming languages</span>
			<div class="GroupContainer">
				<Item name="Python">
					<Python />
				</Item>
				<Item name="Javascript" learning={true}>
					<Js />
				</Item>
				<Item name="Typescript" learning={true}>
					<Ts />
				</Item>
			</div>
		</div>
		<div class="Group">
			<span class="Title">Frameworks and libraries</span>
			<div class="GroupContainer">
				<Item name="Django">
					<Django />
				</Item>
				<Item name="Nest Js" learning={true}>
					<Nest />
				</Item>
				<Item name="Svelte Kit" learning={true}>
					<Svelte />
				</Item>
			</div>
		</div>
		<div class="Group">
			<span class="Title">Other technologies</span>
			<div class="GroupContainer">
				<Item name="Git">
					<Git />
				</Item>
				<Item name="Markdown">
					<Md />
				</Item>
			</div>
		</div>
		<a href="https://github.com/Umatriz" class="Btn">My GitHub</a>
	</div>
</section>

<style>
	.Skills {
		width: 100%;
		height: 100vh;
		display: flex;
		justify-content: center;
		align-items: flex-start;
		flex-direction: column;
	}
	.List {
		display: flex;
		flex-direction: column;
		align-items: flex-start;
		justify-content: flex-start;
	}
	.Group {
		display: flex;
		flex-direction: column;
		align-items: flex-start;
		justify-content: flex-start;
		margin-bottom: 1.5rem;
	}
	.Title {
		font-size: 1.5rem;
		margin-bottom: 0.5rem;
		font-weight: 500;
	}
	.GroupContainer {
		position: relative;
		padding-left: 1.5rem;
		display: flex;
		flex-direction: column;
		align-items: flex-start;
		justify-content: flex-start;
		gap: 0.5rem;
	}
	.GroupContainer::before {
		content: '';
		position: absolute;
		left: 0;
		top: 0;
		height: 100%;
		width: 4px;
		background-color: #1a132f;
		border-radius: 5px;
	}
	.Btn {
		padding: 0.5rem 5rem;
		background-color: #1a132f;
		color: #fff;
		text-decoration: none;
		border-radius: 0.3rem;
	}
</style>
