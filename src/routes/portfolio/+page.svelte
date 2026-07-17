<script lang="ts">
	import Footer from "$lib/assets/Footer.svelte";
	import Navbar from "$lib/assets/Navbar.svelte";
	import ProjectCard from "$lib/assets/ProjectCard.svelte";
	import { onMount } from "svelte";
    let sitePath: string = $state("");

    onMount(() => {
        sitePath = window.location.pathname;
    });
</script>

<div class="main-wrapper">
    <Navbar />
    <div class="gap-6 grid grid-cols-1 md:grid-cols-2 pt-20">
        <ProjectCard title="" description="" imageSrc="" tags={[]} />
        <ProjectCard title="" description="" imageSrc="" tags={[]} />
        <ProjectCard title="" description="" imageSrc="" tags={[]} />
    </div>
    <Footer />
</div>