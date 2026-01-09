<script lang="ts">
	import './layout.css';
	import favicon from '$lib/assets/favicon.svg';
	import { page } from '$app/stores';
	import Header from '$lib/components/Header.svelte';
  	import Footer from '$lib/components/Footer.svelte';

	let { children } = $props();
</script>


<svelte:head><link rel="icon" href={favicon} /></svelte:head>
<div class="mx-auto w-full max-w-[1157px] bg-white">
	<Header />
	{@render children()}

	<Footer />
</div>
