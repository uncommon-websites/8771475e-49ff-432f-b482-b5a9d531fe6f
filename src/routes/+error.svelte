<script lang="ts">
	import { page } from "$app/state";
</script>

<main class="min-h-screen flex items-center justify-center bg-white">
	<div class="text-center">
		<svg width="64" height="64" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" class="w-16 h-16 text-[--color-brand-blue] mx-auto mb-8">
			<path d="M12 2L13.2 9.92154L20.6603 7L14.4 12L20.6603 17L13.2 14.0785L12 22L10.8 14.0785L3.33975 17L9.6 12L3.33975 7L10.8 9.92154L12 2Z" fill="currentColor"/>
		</svg>
		<h1 class="text-6xl font-light text-gray-900 mb-4">{page.status}</h1>
		<p class="text-lg text-gray-600 mb-8">{page.error?.message ?? "Something went wrong."}</p>
		<a href="/" class="inline-flex items-center gap-3 text-[--color-brand-blue] text-sm font-medium hover:opacity-80 transition-opacity">
			<div class="w-8 h-8 border border-[--color-brand-blue] rounded-full flex items-center justify-center">
				<svg width="12" height="12" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
					<path d="M19 12H5M5 12L12 19M5 12L12 5" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
				</svg>
			</div>
			Return Home
		</a>
	</div>
</main>
