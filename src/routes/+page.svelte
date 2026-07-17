<script lang="ts">
	import Footer from "$lib/assets/Footer.svelte";
	import Navbar from "$lib/assets/Navbar.svelte";
	import { onMount } from "svelte";
    let sitePath: string = $state("");

    onMount(() => {
        sitePath = window.location.pathname;
    });
</script>

<div class="main-wrapper">
    <Navbar />
    <div class="main-content center-content">
        <p class="text-5xl text-text-light font-bold">{sitePath}</p>
    </div>
    <Footer />
</div>