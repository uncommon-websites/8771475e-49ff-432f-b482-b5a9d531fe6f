<script lang="ts">
	import { page } from '$app/state';
</script>

<header class="fixed top-0 left-0 w-full z-50 py-8 pointer-events-none">
	<div class="container flex flex-col items-center relative pointer-events-auto">
		<!-- Logo (Top Left) -->
		<a href="/" class="absolute left-6 top-0 text-black hover:opacity-70 transition-opacity">
			<svg width="40" height="40" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" class="w-10 h-10">
				<path d="M12 2L13.2 9.92154L20.6603 7L14.4 12L20.6603 17L13.2 14.0785L12 22L10.8 14.0785L3.33975 17L9.6 12L3.33975 7L10.8 9.92154L12 2Z" fill="currentColor"/>
			</svg>
		</a>

		<!-- Nav -->
		<nav class="hidden md:flex items-center gap-1 bg-[#F4F4F4] px-1.5 py-1.5 rounded-full">
			{#each ['Technology', 'Science', 'Mission', 'Updates', 'Join Us'] as item}
				<a href="#" class="px-5 py-2 text-[13px] font-medium text-gray-600 hover:bg-white hover:shadow-sm rounded-full transition-all">{item}</a>
			{/each}
		</nav>

		<!-- Search/Notification Pill -->
		<div class="hidden lg:flex items-center gap-3 bg-[#F4F4F4] rounded-full pl-5 pr-1.5 py-1.5 mt-2">
			<span class="text-[11px] text-gray-500 tracking-wide font-medium">Transform your species. Break your limits.</span>
			<div class="w-8 h-4 bg-gray-200 rounded-full relative cursor-pointer flex items-center px-0.5">
				<div class="w-3 h-3 bg-[--color-brand-blue] rounded-full shadow-sm ml-auto"></div>
			</div>
		</div>
	</div>
</header>
