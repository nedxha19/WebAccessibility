<script>
	// Svelte logic can be added here
</script>

<div class="min-h-screen bg-gradient-to-br from-gray-900 to-black">
	<!-- Hero Section -->
	<header class="relative overflow-hidden bg-gray-900 py-24">
		<div class="absolute inset-0">
			<img
				src="https://images.unsplash.com/photo-1555949963-ff9fe0c870eb?ixlib=rb-1.2.1&auto=format&fit=crop&w=1920&q=80"
				alt="Code audit visualization"
				class="h-full w-full object-cover opacity-20"
			/>
		</div>
		<div class="container relative mx-auto px-6 text-center">
			<h1 class="mb-4 text-4xl font-bold text-white">Automated Accessibility Testing</h1>
			<p class="mx-auto max-w-3xl text-xl text-orange-400">
				Master WCAG compliance through systematic auditing and remediation
			</p>
		</div>
	</header>

	<main class="container mx-auto px-6 py-12">
		<!-- Testing Process -->
		<section class="mb-16 rounded-2xl bg-gray-800 p-8 shadow-xl">
			<div class="mb-8 flex items-center">
				<div class="mr-4 rounded-lg bg-orange-500 p-3">
					<svg class="h-6 w-6 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
						<path
							stroke-linecap="round"
							stroke-linejoin="round"
							stroke-width="2"
							d="M13 10V3L4 14h7v7l9-11h-7z"
						/>
					</svg>
				</div>
				<h2 class="text-2xl font-semibold text-white">Three-Phase Testing Methodology</h2>
			</div>
			<div class="grid gap-8 md:grid-cols-3">
				<div class="rounded-xl border-l-4 border-orange-500 bg-gray-700 p-6">
					<h3 class="mb-3 text-lg font-semibold text-white">Automated Scanning</h3>
					<p class="text-gray-300">Rapid initial assessment using AI-powered tools</p>
				</div>
				<div class="rounded-xl border-l-4 border-orange-500 bg-gray-700 p-6">
					<h3 class="mb-3 text-lg font-semibold text-white">Manual Verification</h3>
					<p class="text-gray-300">Human evaluation of complex interactions</p>
				</div>
				<div class="rounded-xl border-l-4 border-orange-500 bg-gray-700 p-6">
					<h3 class="mb-3 text-lg font-semibold text-white">AT Validation</h3>
					<p class="text-gray-300">Screen reader & assistive tech testing</p>
				</div>
			</div>
		</section>

		<!-- Audit Demo -->
		<section class="mb-16 rounded-2xl bg-gray-800 p-8 shadow-xl">
			<h2 class="mb-8 flex items-center text-2xl font-semibold text-white">
				<svg
					class="mr-2 h-6 w-6 text-orange-500"
					fill="none"
					stroke="currentColor"
					viewBox="0 0 24 24"
				>
					<path
						stroke-linecap="round"
						stroke-linejoin="round"
						stroke-width="2"
						d="M10 20l4-16m4 4l4 4-4 4M6 16l-4-4 4-4"
					/>
				</svg>
				Lighthouse Audit Walkthrough
			</h2>

			<div class="space-y-8">
				<div class="grid items-start gap-8 md:grid-cols-2">
					<ol class="space-y-6 text-gray-300">
						<li class="flex items-start">
							<span
								class="mr-3 flex h-6 w-6 items-center justify-center rounded-full bg-orange-500 text-white"
								>1</span
							>
							Install Lighthouse via Chrome DevTools
						</li>
						<li class="flex items-start">
							<span
								class="mr-3 flex h-6 w-6 items-center justify-center rounded-full bg-orange-500 text-white"
								>2</span
							>
							Configure accessibility audit settings
						</li>
						<li class="flex items-start">
							<span
								class="mr-3 flex h-6 w-6 items-center justify-center rounded-full bg-orange-500 text-white"
								>3</span
							>
							Analyze page load and review score
						</li>
						<li class="flex items-start">
							<span
								class="mr-3 flex h-6 w-6 items-center justify-center rounded-full bg-orange-500 text-white"
								>4</span
							>
							Implement recommended fixes
						</li>
					</ol>
					<div class="overflow-hidden rounded-lg border-4 border-gray-700">
						<img
							src="https://images.unsplash.com/photo-1555949963-ff9fe0c870eb?ixlib=rb-1.2.1&auto=format&fit=crop&w=1000&q=80"
							alt="Lighthouse audit interface"
							class="h-auto w-full"
						/>
					</div>
				</div>
			</div>
		</section>

		<!-- Common Issues -->
		<section class="mb-16 rounded-2xl bg-gray-800 p-8 shadow-xl">
			<h2 class="mb-8 text-2xl font-semibold text-white">Critical Accessibility Fixes</h2>

			<div class="grid gap-8 md:grid-cols-2">
				<!-- ARIA Roles -->
				<div class="rounded-xl bg-gray-700 p-6">
					<h3 class="mb-4 text-lg font-semibold text-white">ARIA Roles</h3>
					<div class="space-y-4">
						<div>
							<p class="mb-2 text-sm text-orange-400">Issue:</p>
							<code class="block overflow-x-auto rounded bg-gray-900 p-4 text-red-400">
								&lt;button role="list" type="submit"&gt;Subscribe&lt;/button&gt;
							</code>
						</div>
						<div>
							<p class="mb-2 text-sm text-orange-400">Solution:</p>
							<code class="block overflow-x-auto rounded bg-gray-900 p-4 text-green-400">
								&lt;button type="submit"&gt;Subscribe&lt;/button&gt;
							</code>
						</div>
					</div>
				</div>

				<!-- Color Contrast -->
				<div class="rounded-xl bg-gray-700 p-6">
					<h3 class="mb-4 text-lg font-semibold text-white">Color Contrast</h3>
					<div class="flex items-center space-x-4">
						<div class="w-1/2">
							<div class="h-24 rounded bg-white p-2">
								<div class="h-full bg-[#01aa9d]"></div>
							</div>
							<p class="mt-2 text-center text-gray-300">2.9:1 (Fail)</p>
						</div>
						<svg
							class="h-6 w-6 text-orange-500"
							fill="none"
							stroke="currentColor"
							viewBox="0 0 24 24"
						>
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								stroke-width="2"
								d="M14 5l7 7m0 0l-7 7m7-7H3"
							/>
						</svg>
						<div class="w-1/2">
							<div class="h-24 rounded bg-white p-2">
								<div class="h-full bg-[#008576]"></div>
							</div>
							<p class="mt-2 text-center text-gray-300">4.5:1 (Pass)</p>
						</div>
					</div>
				</div>

				<!-- Add other issues similarly -->
			</div>
		</section>

		<!-- Full Fix List -->
		<section class="rounded-2xl bg-gray-800 p-8 shadow-xl">
			<h2 class="mb-8 text-2xl font-semibold text-white">Complete Remediation Guide</h2>
			<div class="space-y-8">
				<div class="border-l-4 border-orange-500 pl-6">
					<h3 class="mb-2 text-lg font-semibold text-white">List Structure</h3>
					<div class="grid gap-4 md:grid-cols-2">
						<code class="overflow-x-auto rounded bg-gray-900 p-4 text-red-400">
							&lt;div class="ul"&gt;...&lt;/div&gt;
						</code>
						<code class="overflow-x-auto rounded bg-gray-900 p-4 text-green-400">
							&lt;ul&gt;...&lt;/ul&gt;
						</code>
					</div>
				</div>

				<!-- Repeat for other issues -->
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

<style>
	/* Custom styles can be added here if needed */
</style>
