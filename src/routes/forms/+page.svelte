<script>
	// Add any necessary Svelte logic here
</script>

<div class="min-h-screen bg-gradient-to-br from-black to-gray-900">
	<!-- Hero Section -->
	<header class="relative overflow-hidden bg-black">
		<div class="absolute inset-0 z-0">
			<img
				src="https://images.unsplash.com/photo-1517694712202-14dd9538aa97"
				alt="Accessible Forms"
				class="h-full w-full object-cover opacity-20"
			/>
		</div>
		<div class="container relative z-10 mx-auto px-6 py-32">
			<div class="mx-auto max-w-4xl text-center">
				<h1 class="mb-6 text-5xl font-extrabold leading-tight text-white">
					Accessible Form Patterns
				</h1>
				<p class="mb-8 text-xl text-gray-300">
					Creating inclusive data collection experiences through WCAG-compliant form design
				</p>
			</div>

			<!-- Menu Section -->
			
					
			</div>
		
	</header>

	<!-- Main Content -->
	<main class="container mx-auto px-6 py-16">
		<section id="foundations" class="mb-20">
			<h2 class="mb-6 text-4xl font-bold text-orange-500">Form Accessibility Fundamentals</h2>
			<div class="grid gap-8 md:grid-cols-2">
				<div class="rounded-xl bg-gradient-to-b from-gray-800/80 to-gray-900/80 p-8 shadow-xl">
					<h3 class="mb-4 text-2xl font-semibold text-white">Core Principles</h3>
					<ul class="list-disc space-y-4 pl-6 text-gray-300">
						<li>Semantic HTML structure</li>
						<li>Clear visual hierarchy</li>
						<li>Keyboard navigation support</li>
						<li>ARIA when necessary</li>
						<li>Error prevention & recovery</li>
					</ul>
				</div>
				<div class="rounded-xl bg-gradient-to-b from-gray-800/80 to-gray-900/80 p-8 shadow-xl">
					<h3 class="mb-4 text-2xl font-semibold text-white">Component Checklist</h3>
					<ul class="list-disc space-y-4 pl-6 text-gray-300">
						<li>Programmatic labels</li>
						<li>Focus management</li>
						<li>Input validation</li>
						<li>Error messaging</li>
						<li>Autocomplete support</li>
					</ul>
				</div>
			</div>
		</section>

		<section id="fields" class="mb-20">
			<h2 class="mb-6 text-4xl font-bold text-orange-500">Field Implementation</h2>
			<div class="grid gap-8 md:grid-cols-2">
				<div class="rounded-xl bg-gray-800/50 p-6 shadow-xl">
					<h3 class="mb-4 text-xl font-semibold text-white">Anti-Pattern</h3>
					<code class="block overflow-x-auto rounded bg-gray-900 p-4 text-red-400">
						&lt;div role="form" id="bad-form"&gt; &lt;span&gt;Name:&lt;/span&gt; &lt;div
						class="input"&gt;&lt;/div&gt; &lt;/div&gt;
					</code>
					<p class="mt-4 text-gray-300">Custom elements without proper semantics</p>
				</div>
				<div class="rounded-xl bg-gray-800/50 p-6 shadow-xl">
					<h3 class="mb-4 text-xl font-semibold text-white">Recommended Pattern</h3>
					<code class="block overflow-x-auto rounded bg-gray-900 p-4 text-green-400">
						&lt;form id="good-form"&gt; &lt;label&gt; Name: &lt;input type="text"
						autocomplete="name"&gt; &lt;/label&gt; &lt;/form&gt;
					</code>
					<p class="mt-4 text-gray-300">Semantic HTML with autocomplete attributes</p>
				</div>
			</div>
		</section>

		<section id="validation" class="mb-20">
			<h2 class="mb-6 text-4xl font-bold text-orange-500">Validation & Errors</h2>
			<div class="grid gap-8 md:grid-cols-2 lg:grid-cols-3">
				<div class="rounded-xl bg-gradient-to-b from-gray-800/80 to-gray-900/80 p-8 shadow-xl">
					<h3 class="mb-4 text-xl font-semibold text-white">Real-Time Validation</h3>
					<p class="text-gray-300">Inline error messages with aria-live regions</p>
					<code class="mt-4 block rounded bg-gray-900 p-4 text-sm text-orange-400">
						aria-live="polite"
					</code>
				</div>
				<div class="rounded-xl bg-gradient-to-b from-gray-800/80 to-gray-900/80 p-8 shadow-xl">
					<h3 class="mb-4 text-xl font-semibold text-white">Error Summary</h3>
					<p class="text-gray-300">Top-of-form error list with anchor links</p>
					<code class="mt-4 block rounded bg-gray-900 p-4 text-sm text-orange-400">
						&lt;div role="alert"&gt;&lt;/div&gt;
					</code>
				</div>
				<div class="rounded-xl bg-gradient-to-b from-gray-800/80 to-gray-900/80 p-8 shadow-xl">
					<h3 class="mb-4 text-xl font-semibold text-white">Input States</h3>
					<p class="text-gray-300">Visual and programmatic error indication</p>
					<code class="mt-4 block rounded bg-gray-900 p-4 text-sm text-orange-400">
						aria-invalid="true"
					</code>
				</div>
			</div>
		</section>

		<section id="complex-forms" class="mb-20">
			<h2 class="mb-6 text-4xl font-bold text-orange-500">Advanced Patterns</h2>
			<div class="rounded-xl bg-gray-800/50 p-8 shadow-xl">
				<div class="grid gap-8 md:grid-cols-2">
					<div>
						<h3 class="mb-4 text-xl font-semibold text-white">Fieldset Grouping</h3>
						<code class="block overflow-x-auto rounded bg-gray-900 p-4 text-green-400">
							&lt;fieldset&gt; &lt;legend&gt;Payment Info&lt;/legend&gt; &lt;!-- Fields --&gt;
							&lt;/fieldset&gt;
						</code>
					</div>
					<div>
						<h3 class="mb-4 text-xl font-semibold text-white">Multi-Step Forms</h3>
						<code class="block overflow-x-auto rounded bg-gray-900 p-4 text-green-400">
							&lt;div role="progressbar" aria-valuenow="25"&gt;&lt;/div&gt;
						</code>
					</div>
				</div>
			</div>
		</section>

		<section id="best-practices" class="mb-20">
			<h2 class="mb-6 text-4xl font-bold text-orange-500">Optimization Techniques</h2>
			<div class="rounded-xl bg-gray-800/50 p-8 shadow-xl">
				<div class="grid gap-8 md:grid-cols-2">
					<div>
						<h3 class="mb-4 text-xl font-semibold text-white">Autocomplete Attributes</h3>
						<code class="block overflow-x-auto rounded bg-gray-900 p-4 text-green-400">
							&lt;input autocomplete="bday"&gt;
						</code>
						<p class="mt-4 text-gray-300">Enhances AT support and user convenience</p>
					</div>
					<div>
						<h3 class="mb-4 text-xl font-semibold text-white">Required Fields</h3>
						<code class="block overflow-x-auto rounded bg-gray-900 p-4 text-green-400">
							&lt;input aria-required="true"&gt;
						</code>
						<p class="mt-4 text-gray-300">Clear indication for screen readers</p>
					</div>
				</div>
			</div>
		</section>
	</main>

	<footer class="mt-16 bg-gradient-to-r from-orange-600 to-orange-700 py-8 text-white">
		<div class="container mx-auto px-6 text-center">
			<p class="mb-2 text-orange-100">© 2025 Nedit Xhaferi. Web Accessibility.</p>
			<p class="text-sm text-orange-200">Commitment to inclusive digital experiences</p>
		</div>
	</footer>
</div>
