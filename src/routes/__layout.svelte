<script>
	import '../app.css';
</script>

<main>
	<slot />
</main>

<style>
	main {
		width: 1000px;
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		margin: 0 auto;
	}
</style>
