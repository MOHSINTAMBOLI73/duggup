<script>
	import Header from '$lib/components/Header.svelte';
	import './style.css';
</script>

<Header />
<slot />

<style>
	:global(body) {
		font-family: 'Inter', sans-serif;
		background-color: #fcfcff;
	}
</style>
