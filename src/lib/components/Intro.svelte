<script>
	export let buttonText = 'Follow';
	function follow() {
		if (buttonText == 'Follow') {
			buttonText = 'Followed';
		} else {
			buttonText = 'Follow';
		}
	}
</script>

<div
	class="mt-10 flex flex-row items-center justify-center lg:space-x-4 xl:space-x-12 2xl:space-x-16"
>
	<div class="text-center">
		<img class="md:w-20 lg:w-24" src="/icons/profile.png" alt="" />
		<p class="font-bold text-[#4B5C6D] md:text-base lg:text-xl">Krishna <br />Kiran</p>
	</div>

	<div class="md:w-[24rem] lg:w-[32rem] xl:w-[42rem] 2xl:w-[48rem]">
		<p class="md:text-xs lg:text-sm">
			Co-Founder and CEO at Duggup - Social network for people in tech. Ex-Amazon Head of
			Engineering. I write hot-takes on building a business, shipping delightful products and
			accelerating product and career growth.
		</p>

		<button
			on:click={follow}
			class="mt-6 flex flex-row items-center rounded border-[0.5px] border-b-4 border-[#4D4D4D] bg-white px-6 py-1 hover:border-[#0066FF] hover:bg-[#0066FF] hover:text-white md:text-xs lg:text-sm"
		>
			{buttonText}
		</button>
	</div>
	<div class="flex flex-col items-end">
		<img class="w-8 cursor-pointer" src="/icons/Logo round.svg" alt="" />
		<h2 class="cursor-pointer font-bold">Duggup</h2>
		<p class="text-xs text-[#7A9299]">Co-Founder and CEO</p>
		<div class="mt-6 flex flex-row space-x-2 text-xs">
			<p>My website</p>
			<img class="cursor-pointer" src="icons/links.svg" alt="" />
			<img class="cursor-pointer" src="icons/dots.svg" alt="" />
		</div>
	</div>
</div>
