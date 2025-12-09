<script lang="ts">
	import Header from "$lib/Header.svelte";
	import Card from "$lib/Card.svelte";

	const cards = [
		{ label: "Brand", type: "brand" },
		{ label: "Snippets", type: "snippets" },
		{ label: "Website", type: "website" },
		{ label: "Ads", type: "ads" },
		{ label: "Deck", type: "deck" }
	];
</script>

<div class="min-h-screen bg-white flex flex-col items-center pb-20">
	<Header />

	<main class="w-full max-w-[1400px] px-6 flex flex-col items-center mt-20 md:mt-32">
		<!-- Hero Text -->
		<h1 class="text-[56px] md:text-[72px] font-bold tracking-tighter leading-[1.1] text-center mb-12">
			<span class="text-black block">Design your company.</span>
			<span class="text-gray-500 block">Sell, hire, raise more.</span>
		</h1>

		<!-- Input Field -->
		<div class="relative w-full max-w-[560px] mb-32">
			<div class="absolute inset-0 bg-gray-200/50 rounded-full blur-2xl transform translate-y-4"></div>
			<div class="relative bg-white rounded-full shadow-[0_8px_30px_rgba(0,0,0,0.04)] border border-gray-100 p-2 flex items-center">
				<input 
					type="text" 
					placeholder="Describe your company..." 
					class="flex-1 bg-transparent border-none outline-none px-6 text-lg placeholder:text-gray-400 text-gray-800 h-12"
				/>
				
				<div class="flex items-center gap-3 pr-2">
					<!-- Paperclip Icon -->
					<button class="text-gray-400 hover:text-gray-600 transition-colors p-2">
						<svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
							<path d="M21.44 11.05l-9.19 9.19a6 6 0 0 1-8.49-8.49l9.19-9.19a4 4 0 0 1 5.66 5.66l-9.2 9.19a2 2 0 0 1-2.83-2.83l8.49-8.48"></path>
						</svg>
					</button>

					<!-- Submit Button -->
					<button class="bg-gray-900 hover:bg-black text-white rounded-full w-10 h-10 flex items-center justify-center transition-colors">
						<svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
							<line x1="12" y1="19" x2="12" y2="5"></line>
							<polyline points="5 12 12 5 19 12"></polyline>
						</svg>
					</button>
				</div>
			</div>
		</div>

		<!-- Cards Grid -->
		<div class="grid grid-cols-2 md:grid-cols-3 lg:grid-cols-5 gap-6 w-full">
			{#each cards as card}
				<Card label={card.label} type={card.type} />
			{/each}
		</div>
	</main>
</div>

