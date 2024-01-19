<script>
	import banner from '$lib/assets/images/image-omelette.jpeg';
</script>

<main>
	<img class="banner" src={banner} alt="Simple Omelette" />
	<article>
		<section class="overview">
			<h1>Simple Omelette Recipe</h1>
			<p>
				An easy and quick dish, perfect for any meal. This classic omelette combines beaten eggs
				cooked to perfection, optionally filled with yolur choice of cheese, vegetables, or meats.
			</p>

			<div class="preparation">
				<h3>Preparation time</h3>
				<ul>
					<li><p><span>Total:</span> Approximately 10 minutes</p></li>
					<li><p><span>Preparation:</span> 5 minutes</p></li>
					<li><p><span>Cooking:</span> 5 minutes</p></li>
				</ul>
			</div>
		</section>

		<section class="ingredients">
			<h2>Ingredients</h2>
			<ul>
				<li><p>2-3 large eggs</p></li>
				<li><p>Salt, to taste</p></li>
				<li><p>Pepper, to taste</p></li>
				<li><p>1 tablespoon of butter or oil</p></li>
				<li><p>Optional fillings: cheese, diced vegetables, cooked meats, herbs</p></li>
			</ul>
		</section>

		<section class="instructions">
			<h2>Instructions</h2>
			<ol>
				<li>
					<p>
						<span>Beat the eggs:</span> In a bowl, beat the eggs with a pinch of salt and pepper until
						they are well mixed. You can add a tablespoon of water or milk for a fluffier texture.
					</p>
				</li>
				<li>
					<p>
						<span>Heat the pan:</span> Place a non-stick frying pan over medium heat and add butter or
						oil
					</p>
				</li>
				<li>
					<p>
						<span>Cook the omelette:</span> Once the butter is melted and bubbling, pour in the eggs.
						Tilt the pan to ensure the eggs evenly coat the surface.
					</p>
				</li>
				<li>
					<p>
						<span>Add fillings (optional): </span>When the eggs begin to set at the edges but are
						still slightly runny in the middle, sprinkle your chosen fillings over one half of the
						omelette.
					</p>
				</li>
				<li>
					<p>
						<span>Fold and serve:</span> As the omelette continues to cook, carefully lift one edge and
						fold it over the fillings.Let it cook for another minute, then slide it onto a plate.
					</p>
				</li>
				<li><p><span>Enjoy:</span> Serve hot, with additional salt and pepper if needed.</p></li>
			</ol>
		</section>

		<section class="nutrition">
			<h2>Nutrition</h2>
			<p>The table below shows nutritional values per serving without the additional fillings</p>
			<table>
				<tr>
					<td>Calories</td>
					<td>277kcal</td>
				</tr>
				<tr>
					<td>Carbs</td>
					<td>0g</td>
				</tr>
				<tr>
					<td>Protein</td>
					<td>20g</td>
				</tr>
				<tr>
					<td>Fat</td>
					<td>22g</td>
				</tr>
			</table>
		</section>
	</article>
</main>

<style>
	/* Layout */
	main {
		max-width: 60rem;
		background-color: var(--clr-neutral-1);
		margin-inline: auto;
	}

  @media(width >= 640px) {
    main {
      padding: 2rem;
      border-radius: 2rem;
      margin-block: 4rem;
      margin-inline: 2rem;
    }
    img {
      border-radius: 1rem;
    }
  }

	article {
		padding: 2rem;
		display: grid;
		gap: 1rem;
	}

	.preparation {
		background-color: var(--clr-neutral-2);
    display: grid;
    gap: 1rem;
		padding: 1rem;
	}

	section {
		display: grid;
		gap: 1rem;
	}

	ul,
	ol {
		padding-inline: 1rem;
		text-align: start;
		display: grid;
		gap: 1rem;
		/* border-bottom: 1px solid var(--clr-neutral-4); */
		/* text-indent: 1rem; */
	}

	/* Component */

	.ingredients,
	.instructions {
		border-bottom: 1px solid var(--clr-neutral-4);
		padding-bottom: 1rem;
	}

	table {
		border-collapse: collapse;
	}

	tr {
		/* border: 1px solid red; */
		border-bottom: 1px solid var(--clr-neutral-4);
		/* padding: 1rem; */
		line-height: 2.5rem;
		text-indent: 2rem;
	}

	/* Typography */

	ol > li::marker {
		font-weight: var(--fw-bold);
	}

	li > p {
		margin-left: 1rem;
	}

	h1 {
		font-family: var(--ff-primary-1);
		color: var(--clr-neutral-6);
		font-size: xx-large;
	}

	h2 {
		color: var(--clr-primary-1);
		font-size: x-large;
	}

  h3 {
    color: var(--clr-primary-2);
    font-family: var(--ff-primary-2);
  }

	p {
		color: var(--clr-neutral-6);
		line-height: 1.5rem;
		vertical-align: bottom;
	}

	span {
		font-weight: var(--fw-bold);
	}

	tr > td:nth-child(2) {
		font-weight: var(--fw-bold);
	}
</style>
