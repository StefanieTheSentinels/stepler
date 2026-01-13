<script lang="ts">
	import './layout.css';
	import favicon from '$lib/assets/favicon.svg';
	import Header from '$lib/components/Header.svelte';
  	import Footer from '$lib/components/Footer.svelte';
	import Courses from '$lib/components/Courses.main.svelte';

	let { children } = $props();
</script>


<svelte:head><link rel="icon" href={favicon} /></svelte:head>
<div class="mx-auto w-full max-w-[1157px] bg-white">
	<Header />
	{@render children()}
	
	<Courses />

	<Footer />
</div>
