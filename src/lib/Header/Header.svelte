<section class="Container">
	<h1 class="Title">Umatriz</h1>
	<span class="WebDev">Web Developer</span>
	<a href="#skills" class="SkillsBtn">Click me!</a>
</section>

<style>
	.Container {
		width: 100%;
		height: 100vh;
		display: flex;
		align-items: center;
		justify-content: center;
		flex-direction: column;
		gap: 0.5rem;
	}
	.Title {
		font-size: 15rem;
		line-height: 1;
		font-weight: 700;
		background: url('./leaves.jpg') no-repeat;
		background-clip: text;
		-webkit-background-clip: text;
		color: transparent;
		animation: moveBg 15s linear infinite;
		-webkit-animation: moveBg 15s linear infinite;
	}
	@keyframes moveBg {
		0% {
			background-position: 0% 0%;
		}
		100% {
			background-position: 100% 100%;
		}
	}
	.WebDev {
		font-size: 3rem;
		font-weight: 400;
		width: 13ch;
		animation: typing 2s steps(13), blink 0.5s step-end infinite alternate;
		white-space: nowrap;
		overflow: hidden;
		border-right: 3px solid;
	}

	@keyframes typing {
		from {
			width: 0;
		}
	}

	@keyframes blink {
		50% {
			border-color: transparent;
		}
	}
	.SkillsBtn {
		padding: 0.5rem 5rem;
		background-color: #1a132f;
		color: #fff;
		text-decoration: none;
		border-radius: 0.3rem;
	}
</style>
