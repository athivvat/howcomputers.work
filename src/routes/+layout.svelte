<script lang="ts">
	import '../app.css';
	import Footer from '../components/Footer.svelte';
	let { children } = $props();
</script>

<div class="relative">
	<!-- Left Stripe -->
	<div class="stripe-pattern absolute lg:left-[402px] left-4 top-0 h-full w-[46px]"></div>

	<!-- Right Stripe -->
	<div class="stripe-pattern absolute lg:right-[402px] right-4 top-0 h-full w-[46px]"></div>
	
	{@render children()}

	<Footer />
</div>
