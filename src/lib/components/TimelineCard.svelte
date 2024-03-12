<script>
	export let month = '';
	export let year = '';
	export let imageUrl = '';
	export let imageUrl1 = '';
	export let description = '';
	export let description1 = '';
</script>

<div class="flex items-center space-x-8">
	<div class="w-[8.5rem] text-right">
		<p class="text-xs text-[#7A9299]">{month} {year}</p>
	</div>
	<div class="flex h-52 items-center">
		<div class="h-3 w-3 rounded-full border-2 border-[#0066FF] bg-white"></div>
	</div>
	<div
		class="flex h-40 w-64 flex-col items-center overflow-hidden rounded-lg border border-gray-300"
	>
		<img class="h-24 w-full object-cover object-center" src={imageUrl} alt="" />
		<p class="overflow-hidden bg-white p-4 text-xs">{description}</p>
	</div>
	<div
		class="flex h-40 w-64 flex-col items-center overflow-hidden rounded-lg border border-gray-300"
	>
		<img class="h-24 w-full object-cover object-center" src={imageUrl1} alt="" />
		<p class="overflow-hidden bg-white p-4 text-xs">{description1}</p>
	</div>
</div>
