<script>
	export let compIcon = '';
	export let compName = '';
	export let city = '';
	export let month = '';
	export let year = '';
	export let compHeading = '';
	export let jobType = '';
	export let jobMode = '';
</script>

<div class="flex items-center space-x-7">
	<div class="flex w-[8.5rem] flex-col items-end">
		<img class="w-10" src={compIcon} alt="" />
		<h2 class="font-bold">{compName}</h2>
		<p class="text-xs text-[#7A9299]">{city}</p>
		<p class="text-xs text-[#7A9299]">Joined</p>
		<p class="text-xs text-[#7A9299]">{month} {year}</p>
	</div>
	<div class="flex h-40 flex-col items-center justify-around">
		<img class="rotate-180" src="\icons\down.svg" alt="" />
		<div class="my-16 h-5 w-5 rounded-full border-[6px] border-[#0066FF] bg-white"></div>
	</div>
	<div class="w-[33rem] bg-white p-3">
		<h1 class="text-lg font-bold">{compHeading}</h1>
		<div class="flex items-center">
			<p class="text-xs text-[#7A9299]">{jobType}</p>
			<p
				class="flex items-center text-xs text-[#7A9299] before:mx-1 before:block before:h-0.5 before:w-0.5 before:rounded-full before:bg-[#7A9299]"
			>
				{jobMode}
			</p>
		</div>
	</div>
</div>
