<script>
	import welcome from '$lib/images/svelte-welcome.webp';
	import welcome_fallback from '$lib/images/svelte-welcome.png';

	var test = ""
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Maaaaafia" />
</svelte:head>

<div class="flex w-full items-center h-screen justify-center">
	<div class="flex flex-col">
		<label for="account-number" class="block text-sm font-medium leading-6 text-gray-900">Rechnungs Nummer</label>
		<div class="relative mt-2 rounded-md shadow-sm">
			<input type="text" name="account-number" id="account-number" bind:value={test} class="block w-full rounded-md border-0 py-1.5 pr-10 text-gray-900 ring-1 ring-inset ring-gray-300 placeholder:text-gray-400 focus:ring-2 focus:ring-inset focus:ring-indigo-600 sm:text-sm sm:leading-6" placeholder="0000">
			<div class="pointer-events-none absolute inset-y-0 right-0 flex items-center pr-3">
			<svg class="h-5 w-5 text-gray-400" viewBox="0 0 20 20" fill="currentColor" aria-hidden="true" data-slot="icon">
				<path fill-rule="evenodd" d="M18 10a8 8 0 1 1-16 0 8 8 0 0 1 16 0ZM8.94 6.94a.75.75 0 1 1-1.061-1.061 3 3 0 1 1 2.871 5.026v.345a.75.75 0 0 1-1.5 0v-.5c0-.72.57-1.172 1.081-1.287A1.5 1.5 0 1 0 8.94 6.94ZM10 15a1 1 0 1 0 0-2 1 1 0 0 0 0 2Z" clip-rule="evenodd" />
			</svg>
	
			
		</div>
		{#if test == "1979"}
			<p>
				Taxi Ziel:
				Bakerstreet 69
			</p>
		{/if}
	  </div>
	</div>
</div>