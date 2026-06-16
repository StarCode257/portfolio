<script>
	import * as Card from '$lib/components/ui/card';
</script>

<main class="p-4">
	<!-- salutation section -->
	<section>
		<h1 class="scroll-m-20 text-4xl font-extrabold tracking-tight lg:text-5xl">
			Hey there, I'm Diamant
		</h1>
		<span>
			I'm an <b>application developer</b> skilled in designing and building modern, <br />
			feature-rich applications with a focus on usability, performance and security. <br />
			Passionate about solving problems with technology and <br />
			continuously learning new tools and frameworks.
		</span>
		<br />
		<br />
		<br />
		<br />

		<span>starcode257@gmail.com</span>
	</section>

	<!-- what do i help section  -->
	<section class="flex max-w-200 flex-wrap items-center justify-between">
		<div>
			<h2
				class="scroll-m-20 border-b pb-2 text-3xl font-semibold tracking-tight transition-colors first:mt-0"
			>
				What do I help
			</h2>
			<p>
				I will build a digital solution for you or for your company <br />
				with usable and performant and secured.
			</p>
		</div>
		<div>
			<Card.Root>
				<div class="flex">
					<span>Icon</span>
					<div>
						<h1>Web development</h1>
						<span>Own a website for your company</span>
					</div>
				</div>
			</Card.Root>
			<Card.Root>
				<div class="flex">
					<span>Icon</span>
					<div>
						<h1>Mobile development</h1>
						<span>
							Own an android or ios app <br />
							to manage your company
						</span>
					</div>
				</div>
			</Card.Root>
			<Card.Root>
				<div class="flex">
					<span>Icon</span>
					<div>
						<h1>Desktop development</h1>
						<span>Own tools for your company</span>
					</div>
				</div>
			</Card.Root>
		</div>
	</section>

	<!-- what do i know section  -->
	<section>
		<div>
			<h2
				class="scroll-m-20 border-b pb-2 text-3xl font-semibold tracking-tight transition-colors first:mt-0"
			>
				What do I know
			</h2>
			<p>
				I am a skilled developer using as main tool <br />
				SvelteKit (JavaScript framework) for building web application. <br />
				Flutter for building mobile and Desktop applications. <br />
				Python, FastApi and It's libraries to build AI capabilities <br />
				Rust for building low lever application for your company
			</p>
		</div>
	</section>
</main>
