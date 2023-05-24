<script lang="ts">
	import "../global.css";
	import NL from "$lib/assets/NL.svg?raw";
</script>

<div class="background" />
<div class="container">
	<nav>
		<a href="/">
			{@html NL}
		</a>
		<hr />
		<a href="/books">BOOKS</a>
		<a href="/books">ARTICLES</a>
		<a href="/books">BIO</a>
	</nav>
	<slot />
</div>

<style>
	.background {
		position: absolute;
		top: 0;
		left: 0;
		width: 100vw;
		height: 100vh;
		z-index: -20;

		background: var(--red-0);
	}

	nav {
		display: flex;
		gap: 2rem;
		align-items: center;

		padding: 4rem 0;
	}

	nav hr {
		color: var(--blue-6);

		width: 1.5rem;

		transform: rotate(90deg);
	}

	nav a {
		color: var(--blue-6);
	}

	.container {
		margin: 0 clamp(4rem, 10%, 20rem);
	}
</style>
