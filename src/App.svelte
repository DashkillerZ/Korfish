<script>
	import Header from './components/header.svelte';
	import Page from './components/page.svelte';
	import Page2 from './components/page2.svelte';
	import Footer from './components/footer.svelte';
import BadBots from './components/other/badBots.svelte';
import BadWords from './components/other/badWords.svelte';
import ProxyProtection from './components/other/proxyProtection.svelte';
import SpamProtection from './components/other/spamProtection.svelte';
import SqliProtection from './components/other/sqliProtection.svelte';
	let activePage= 0;
	function handleAnswer(e) {
		activePage= e.detail;
	}

</script>

<main>
	<Header on:handle={handleAnswer}  />
	<main>
		{#if activePage==0}
		<Page/>	
		{:else if activePage==1}
		<BadBots />
		{:else if activePage==2}
		<BadWords/>
		{:else if activePage==3}
		<ProxyProtection />
		{:else if activePage==4}
		<SpamProtection />
		{:else if activePage==5}
		<SqliProtection />
		{/if}
	</main>
	<Footer/>
</main>
 
<style>

</style>