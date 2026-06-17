<script>
	import * as Card from '$lib/components/ui/card';
	import my_image from '$lib/assets/N600-transparent.png';
	import web_app from '$lib/assets/web-app.png';
	import mobile_app from '$lib/assets/mobile-app.png';
	import desktop_app from '$lib/assets/desktop-app.png';
</script>

<main class="mt-24 p-4">
	<!-- hero section -->
	<section class="m-auto flex max-w-6xl flex-wrap justify-between">
		<div>
			<h1 class="scroll-m-20 text-4xl font-extrabold tracking-tight lg:text-5xl">
				Hey there, I'm Diamant
			</h1>
			<p class="leading-7 not-first:mt-6">
				I'm a <b>software developer</b> skilled in designing and building modern, <br />
				feature-rich applications with a focus on usability, performance and security. <br />
				Passionate about solving problems with technology and <br />
				continuously learning new tools and frameworks.
			</p>
			<br />
			<div class="flex items-center gap-2">
				<span><i class="fa fa-envelope"></i></span>
				<span>starcode257@gmail.com</span>
			</div>
		</div>
		<div>
			<img alt="portfolio_image" src={my_image} />
		</div>
	</section>

	<!-- what do i help section  -->
	<section class="m-auto max-w-200">
		<h2
			class="scroll-m-20 border-b pb-2 text-3xl font-semibold tracking-tight transition-colors first:mt-0"
		>
			What do I help
		</h2>
		<p class="leading-7 not-first:mt-6">
			I will build a digital solution for you or for your company with usable, performant and
			secured solutions.
		</p>
		<div class="flex flex-col gap-4">
			<Card.Root>
				<div class="flex items-center gap-4 px-4 md:px-8">
					<img src={web_app} alt="" width="100" />
					<div>
						<h1>Web development</h1>
						<span>Own a website for your company</span>
					</div>
				</div>
			</Card.Root>
			<Card.Root>
				<div class="flex items-center gap-4 px-4 md:px-8">
					<img src={mobile_app} alt="" width="100" />
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
				<div class="flex items-center gap-4 px-4 md:px-8">
					<img src={desktop_app} alt="" width="100" />
					<div>
						<h1>Desktop development</h1>
						<span>Own tools for your company</span>
					</div>
				</div>
			</Card.Root>
		</div>
	</section>

	<br />
	<br />

	<!-- what do i know section  -->
	<section class="m-auto max-w-200">
		<h2
			class="scroll-m-20 border-b pb-2 text-3xl font-semibold tracking-tight transition-colors first:mt-0"
		>
			What do I know
		</h2>
		<p class="leading-7 not-first:mt-6">I am a skilled developer using as main tools :</p>
		<ul class="my-6 ms-6 list-disc [&>li]:mt-2">
			<li>SvelteKit (JavaScript framework) for building web application.</li>
			<li>Flutter for building mobile and Desktop applications.</li>
			<li>Python, FastApi and It's libraries to build AI capabilities</li>
			<li>Rust for building low lever application for your company</li>
		</ul>
	</section>
</main>
