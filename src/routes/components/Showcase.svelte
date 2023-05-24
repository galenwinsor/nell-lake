<script lang="ts">
	export let title: string;
	export let action: string;
	export let destination: string;
	export let side: "left" | "right" | "" = "";
	export let media = "";
</script>

<section style:justify-content={side === "right" ? "flex-end" : ""}>
	{#if side === "left" && media}
		<div class="media">
			<img src={media} alt="title" />
		</div>
	{/if}
	<div class="content" style:max-width={side ? "36rem" : ""}>
		<h2>{title}</h2>
		<slot />
		<a href={destination}>{action} <i class="fa-solid fa-arrow-right" /></a>
		{#if side === "right" && media}
			<div class="media">
				<img src={media} alt="title" />
			</div>
		{/if}
	</div>
</section>

<style>
	section {
		display: flex;
		gap: var(--flex-gap);
		flex-wrap: wrap;
	}

	a {
		display: block;
		margin-top: 1rem;

		color: var(--action);
	}

	h2 {
		margin-bottom: 1rem;
	}

	.media {
		flex-shrink: 0;
		width: 16rem;
	}
</style>
