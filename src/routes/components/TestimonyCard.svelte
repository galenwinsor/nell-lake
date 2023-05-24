<script lang="ts">
	import ted from "$lib/assets/ted.png";
</script>

<div class="card">
	<div class="top-row">
		<div class="image">
			<img src={ted} alt="Mark kramer" />
		</div>
		<div class="title">
			<h3>mark kramer</h3>
			<p class="about">Nieman Foundation, founding editor</p>
		</div>
	</div>
	<div class="content">
		<slot />
	</div>
</div>

<style>
	.card {
		/* glass effect */
		background: rgba(255, 255, 255, 0.2);
		border-radius: 1rem;
		box-shadow: 0 0.25rem 2rem rgba(0, 0, 0, 0.1);
		border: 1px solid rgba(255, 255, 255, 0.3);

		flex-shrink: 1;
		flex-basis: 24rem;

		padding: 2rem;
	}

	.top-row {
		display: flex;
		align-items: center;
		gap: var(--flex-gap);

		margin-bottom: 1rem;
	}

	.image {
		position: relative;

		flex-shrink: 0;
		height: 6rem;
		width: 6rem;

		overflow: hidden;
		border-radius: 100%;
	}

	.image img {
		width: auto;
		height: 100%;

		position: absolute;
		top: 50%;
		left: 50%;
		transform: translateX(-50%) translateY(-50%);
	}
</style>
