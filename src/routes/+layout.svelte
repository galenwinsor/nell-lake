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
		<ul>
			<li>
				<a href="/books">BOOKS</a>
			</li>
			<li>
				<a href="/articles">ARTICLES</a>
			</li>
			<li>
				<a href="/about">BIO</a>
			</li>
		</ul>
	</nav>
	<slot />
	<footer>
		<p>© Nell Lake 2023</p>
		<ul>
			<li>
				<a href="/books">BOOKS</a>
			</li>
			<li>
				<a href="/articles">ARTICLES</a>
			</li>
			<li>
				<a href="/about">ABOUT</a>
			</li>
		</ul>
		<p>Site design by Galen Winsor</p>
	</footer>
</div>

<style>
	.background {
		position: fixed;
		top: 0;
		left: 0;
		width: 100vw;
		height: 100vh;
		z-index: -20;

		background: var(--red-0);
	}

	nav {
		display: flex;
		gap: var(--flex-gap);
		align-items: center;

		padding: 4rem 0;
	}

	nav hr {
		color: var(--blue-6);

		width: 1.5rem;

		transform: rotate(90deg);
	}

	a {
		color: var(--blue-6);
	}

	.container {
		margin: 0 clamp(4rem, 10%, 20rem);
	}

	footer {
		display: flex;
		justify-content: space-between;
		align-items: center;

		padding: 4rem 0;
	}

	ul {
		list-style: none;

		display: flex;
		gap: var(--flex-gap);
	}
</style>
