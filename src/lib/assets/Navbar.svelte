<script lang="ts">
	import { onMount } from "svelte";
    let currentRoute = $state("");

    onMount(() => {
        currentRoute = window.location.pathname;
    });
</script>

<div class="bg-backdrop top-0 w-screen h-40 md:px-80 py-8 flex-col md:flex-row center-content md:justify-between">
    <!-- Title and Email -->
    <div class="w-65 h-full center-content md:m-12">
        <p class="text-gray-300 font-xl font-bold m-1 whitespace-nowrap">Max McDaniel</p>
        
        <div class="w-0.5 h-4 opacity-20 shrink-0 bg-gray-300 m-1"></div>

        <a href="mailto:me@dodoseal.com" id="email-button" class="text-gray-300 font-xl font-bold m-1 hover:underline underline-offset-2 cursor-pointer">me@dodoseal.com</a>
    </div>

    <!-- Navigation Buttons -->
    <div class="w-75 h-full flex center-content">
        <a href="/" class="{currentRoute === "/" ? "text-gray-300" : "text-gray-500"} font-xl font-bold m-4 hover:text-gray-300 transition-colors duration-200 cursor-pointer" id="nav-home">Home</a>
        <a href="/portfolio" class="{currentRoute === "/portfolio" ? "text-gray-300" : "text-gray-500"} font-xl font-bold m-4 hover:text-gray-300 transition-colors duration-200 cursor-pointer" id="nav-portfolio">Portfolio</a>
        <a href="/contact" class="{currentRoute === "/contact" ? "text-gray-300" : "text-gray-500"} font-xl font-bold m-4 hover:text-gray-300 transition-colors duration-200 cursor-pointer" id="nav-contact">Contact</a>
    </div>
</div>