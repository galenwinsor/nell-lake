<h1 class="title">Nell Lake</h1>
<div class="stripe one" />
<div class="stripe two" />
<div class="stripe three" />

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
</style>
