<script lang="ts">
	import headshot from "$lib/assets/headshot.png";
</script>

<section>
	<div class="headshot">
		<img src={headshot} alt="Headshot of Nell Lake" />
	</div>
	<p>
		For more than 20 years, I’ve reported on, analyzed, and written intimate narrative about
		American social issues, focusing on health, healthcare, and medicine. My first book, The
		Caregivers: A Support Group’s Stories of Slow Loss, Courage, and Love, chronicles two years in
		the lives of people caring for ill and elderly family members (Scribner 2014; paperback 2015).
		Since the fall of 2016, I’ve been pursuing a PhD in American Studies at Brown, focusing on the
		politics of care. In AY 2020-2021, I held an American Dissertation Fellowship from the American
		Association of University Women and for three years have been a research associate with the Five
		College Women’s Studies Research Center...
	</p>
</section>

<style>
	.headshot {
		flex-shrink: 0;
		height: 16rem;
		width: 16rem;

		border-radius: 100%;

		overflow: hidden;

		background: var(--brown-1);
	}

	.headshot img {
		width: 88%;

		display: block;

		margin: 0 auto;
	}

	section {
		display: flex;
		gap: var(--flex-gap);
	}
</style>
