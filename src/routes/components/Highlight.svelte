<script lang="ts">
	export let title: string;
</script>

<div>
	<h3>{title}</h3>
	<p>
		<slot />
	</p>
</div>

<style>
	div {
		width: 24rem;
	}

	h3 {
		font-size: 1.5rem;
		letter-spacing: 0.1rem;

		margin-bottom: 1rem;
	}
</style>
