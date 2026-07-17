<script lang="ts">
	import Footer from "$lib/assets/Footer.svelte";
	import Navbar from "$lib/assets/Navbar.svelte";
	import PageTitle from "$lib/assets/PageTitle.svelte";
	import { onMount } from "svelte";
</script>

<div class="main-wrapper">
    <Navbar />
    <PageTitle title="Hey!, I am Max! 👋" description="Some boring stuff that describes who I am and what I do... yeah let's go with that..."/>
    <div class="main-content center-content">
        <!-- Stuff about me goes here btw -->
    </div>
    <Footer />
</div>