<script lang="ts">
	import Footer from "$lib/assets/Footer.svelte";
	import Navbar from "$lib/assets/Navbar.svelte";
	import PageTitle from "$lib/assets/PageTitle.svelte";
	import aboutMe from '$lib/assets/about-me.txt?raw';
</script>

<div class="main-wrapper">
    <Navbar />
    <PageTitle title="Hey, I am Max! 👋" description={aboutMe}/>
    <div class="main-content center-content text-text-light">
        <!-- Stuff about me goes here btw -->
        <p class="text-xl md:text-5xl self-start text-yellow-400 text-center">This website is under construction! Feel free to explore my work at <a class="text-blue-500 underline underline-offset-2" target="_blank" href="https://github.com/dodoseal">https://github.com/dodoseal</a></p>
    </div>
    <Footer />
</div>