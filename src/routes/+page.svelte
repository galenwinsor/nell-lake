<script lang="script">
	import Bio from "./components/Bio.svelte";
	import Highlight from "./components/Highlight.svelte";
	import Showcase from "./components/Showcase.svelte";
	import TestimonyCard from "./components/TestimonyCard.svelte";
	import caregivers from "$lib/assets/caregivers-cover.png";
	import ted from "$lib/assets/ted.png";
</script>

<header>
	<h1 class="title">Nell Lake</h1>
	<div class="stripe one" />
	<div class="stripe two" />
	<div class="stripe three" />
</header>
<section class="highlights">
	<Highlight title="author">
		Lorem ipsum, dolor sit amet consectetur adipisicing elit. Officiis neque consectetur esse vitae
		illum ex dolores enim laborum ratione, quisquam quos nostrum ad fuga eius vero deserunt nemo
		saepe dolore.
	</Highlight>
	<Highlight title="professor">
		Lorem ipsum, dolor sit amet consectetur adipisicing elit. Officiis neque consectetur esse vitae
		illum ex dolores enim laborum ratione, quisquam quos nostrum ad fuga eius vero deserunt nemo
		saepe dolore.
	</Highlight>
	<Highlight title="journalist">
		Lorem ipsum, dolor sit amet consectetur adipisicing elit. Officiis neque consectetur esse vitae
		illum ex dolores enim laborum ratione, quisquam quos nostrum ad fuga eius vero deserunt nemo
		saepe dolore.
	</Highlight>
	<Highlight title="editor & coach">
		Lorem ipsum, dolor sit amet consectetur adipisicing elit. Officiis neque consectetur esse vitae
		illum ex dolores enim laborum ratione, quisquam quos nostrum ad fuga eius vero deserunt nemo
		saepe dolore.
	</Highlight>
</section>
<Bio />
<Showcase
	title="the caregivers"
	action="See all books"
	destination="/books"
	media={caregivers}
	side="left"
>
	<p>
		“[A] beautifully written account of a year in the company of caregivers… The Caregivers is as
		elegantly constructed as a novel, but more than that, Lake writes about these people with such
		warmth and vividness that they feel as memorable as our favorite fictional characters. In
		sharing these stories with readers, Lake has written a book that bears witness to their
		‘necessary, intimate, private heroism.'”
	</p>
	<br />
	<p style:font-weight="bold">The Boston Globe</p>
</Showcase>
<Showcase
	title="health as morality in american life (brown university)"
	action="See all courses"
	destination="/teaching"
	side="right"
>
	<p>
		Lorem ipsum dolor sit amet consectetur adipisicing elit. Error pariatur ea ullam veniam quasi
		suscipit! Tempore ad illum id omnis, provident dignissimos aperiam maiores inventore architecto
		neque necessitatibus numquam quae.
	</p>
	<br />
	<p style:font-weight="bold">Student evaluation</p>
</Showcase>
<Showcase title="praise for my coaching and editing" action="Get in touch" destination="/editing">
	<div class="testimonies">
		<TestimonyCard>
			<p>
				Lorem ipsum dolor, sit amet consectetur adipisicing elit. In nulla ullam repellat expedita
				id iste quam quidem quae quos? Ratione doloremque exercitationem mollitia nostrum inventore.
				Corporis magnam alias possimus. Voluptatem?
			</p>
		</TestimonyCard>
		<TestimonyCard>
			<p>
				Lorem ipsum dolor, sit amet consectetur adipisicing elit. In nulla ullam repellat expedita
				id iste quam quidem quae quos? Ratione doloremque exercitationem mollitia nostrum inventore.
				Corporis magnam alias possimus. Voluptatem?
			</p>
		</TestimonyCard>
		<TestimonyCard>
			<p>
				Lorem ipsum dolor, sit amet consectetur adipisicing elit. In nulla ullam repellat expedita
				id iste quam quidem quae quos? Ratione doloremque exercitationem mollitia nostrum inventore.
				Corporis magnam alias possimus. Voluptatem?
			</p>
		</TestimonyCard>
		<TestimonyCard>
			<p>
				Lorem ipsum dolor, sit amet consectetur adipisicing elit. In nulla ullam repellat expedita
				id iste quam quidem quae quos? Ratione doloremque exercitationem mollitia nostrum inventore.
				Corporis magnam alias possimus. Voluptatem?
			</p>
		</TestimonyCard>
	</div>
</Showcase>

<style>
	.title {
		font-size: 8rem;

		margin-top: 12rem;
	}

	.stripe {
		position: absolute;
		top: -2%;
		z-index: -10;

		width: 12rem;

		border-radius: 1rem;
	}

	.stripe.one {
		right: 20rem;

		height: 24rem;
		width: 12rem;

		border: solid 0.4rem var(--red-3);
	}

	.stripe.two {
		right: 12rem;

		height: 22rem;

		background: var(--blue-2);
	}

	.stripe.three {
		right: 6rem;

		height: 30rem;
		width: 12rem;

		background: var(--brown-2);
	}

	.highlights {
		display: flex;
		flex-wrap: wrap;
		gap: var(--flex-gap);
	}

	.testimonies {
		display: flex;
		flex-wrap: wrap;
		gap: var(--flex-gap);

		width: 100%;
	}
</style>
