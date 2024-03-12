<script>
	import TimelineCard from '$lib/components/TimelineCard.svelte';
	import TimelineCompany from './TimelineCompany.svelte';
	import timelineData from '$lib/timelineData.json';
</script>

<div class="relative m-auto md:w-[53.5rem] lg:w-[63.5rem] xl:w-[77rem] 2xl:w-[85.5rem]">
	<div
		class="absolute left-[10.83rem] -z-10 h-full w-1 border-l-2 border-dotted border-[#778FB1]"
	></div>
	{#each timelineData as item}
		{#if item.type === 'card'}
			<TimelineCard
				month={item.month}
				year={item.year}
				imageUrl={item.imageUrl}
				description={item.description}
				imageUrl1={item.imageUrl1}
				description1={item.description1}
			/>
		{:else if item.type === 'company'}
			<TimelineCompany
				compIcon={item.compIcon}
				compName={item.compName}
				city={item.city}
				month={item.month}
				year={item.year}
				compHeading={item.compHeading}
				jobType={item.jobType}
				jobMode={item.jobMode}
			/>
		{/if}
	{/each}
</div>
