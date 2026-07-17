<script lang="ts">
	import Footer from "$lib/assets/Footer.svelte";
	import Navbar from "$lib/assets/Navbar.svelte";
	import PageTitle from "$lib/assets/PageTitle.svelte";
	import ProjectCard from "$lib/assets/ProjectCard.svelte";
	import { onMount } from "svelte";
    let sitePath: string = $state("");

    onMount(() => {
        sitePath = window.location.pathname;
    });
</script>

<div class="main-wrapper">
    <Navbar />
    <PageTitle title="Projects" description="Description here haha lol idk what to write, just make something up for now yeah... :D"/>
    <div class="gap-6 grid grid-cols-1 md:grid-cols-2 pt-6">
        <ProjectCard title="" description="" imageSrc="" tags={[]} />
        <ProjectCard title="" description="" imageSrc="" tags={[]} />
        <ProjectCard title="" description="" imageSrc="" tags={[]} />
    </div>
    <Footer />
</div>