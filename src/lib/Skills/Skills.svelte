<script>
	import Python from '$lib/Icons/Python.svelte';
	import Js from '$lib/Icons/Js.svelte';
	import Django from '$lib/Icons/Django.svelte';
	import Svelte from '$lib/Icons/Svelte.svelte';
	import Git from '$lib/Icons/Git.svelte';
	import Md from '$lib/Icons/Md.svelte';
</script>

<section class="Skills" id="skills">
	<div class="List">
		<div class="Group">
			<span class="Title">Programming languages</span>
			<div class="GroupContainer">
				<div class="Item">
					<div class="Icon"><Python /></div>
					<span class="Text">Python</span>
				</div>
				<div class="Item">
					<div class="Icon"><Js /></div>
					<span class="Text">Js</span>
				</div>
			</div>
		</div>
		<div class="Group">
			<span class="Title">Frameworks and libraries</span>
			<div class="GroupContainer">
				<div class="Item">
					<div class="Icon"><Django /></div>
					<span class="Text">Django</span>
				</div>
				<div class="Item">
					<div class="Icon"><Svelte /></div>
					<span class="Text">Svelte Kit</span>
				</div>
			</div>
		</div>
		<div class="Group">
			<span class="Title">Other technologies</span>
			<div class="GroupContainer">
				<div class="Item">
					<div class="Icon"><Git /></div>
					<span class="Text">Git</span>
				</div>
				<div class="Item">
					<div class="Icon"><Md /></div>
					<span class="Text">Markdown</span>
				</div>
			</div>
		</div>
	</div>
	<a href="https://github.com/Umatriz" class="Btn">My GitHub</a>
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
	.Item {
		display: flex;
		align-items: center;
		justify-content: center;
	}
	.Icon {
		height: 2rem;
		width: 2rem;
	}
	.Text {
		font-size: 1.3rem;
	}
	.Btn {
		padding: 0.5rem 5rem;
		background-color: #1a132f;
		color: #fff;
		text-decoration: none;
		border-radius: 0.3rem;
	}
</style>
