<script lang="ts">
	import Footer from "$lib/assets/Footer.svelte";
	import Navbar from "$lib/assets/Navbar.svelte";
	import PageTitle from "$lib/assets/PageTitle.svelte";
	import aboutMe from '$lib/assets/about-me.txt?raw';
</script>

<div class="main-wrapper">
    <Navbar />
    <PageTitle title="Hey, I am Max! 👋" description={aboutMe}/>
    <div class="main-content center-content">
        <!-- Stuff about me goes here btw -->
    </div>
    <Footer />
</div>