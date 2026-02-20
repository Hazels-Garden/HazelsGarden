<script lang="ts">
	import favicon from '$lib/assets/hazels-garden.png';
	import Header from './Header.svelte';
	import Footer from './Footer.svelte';
	import './reset.css'
	import './styles.css'
    import { title } from 'process';
	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
	<title>Hazel's Garden LLC</title>
</svelte:head>

<Header/>

<main>
	{@render children()}
</main>

<Footer/>
