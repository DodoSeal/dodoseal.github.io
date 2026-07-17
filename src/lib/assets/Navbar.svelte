<script lang="ts">
	import { onMount } from "svelte";
    let currentRoute = $state("");

    onMount(() => {
        currentRoute = window.location.pathname;
    });
</script>

<div class="bg-backdrop fixed top-0 w-screen md:w-200 h-40 py-8 flex flex-col md:flex-row items-center place-content-center md:justify-between">
    <!-- Title and Email -->
    <div class="w-75 h-full flex center-content">
        <p class="text-gray-300 font-xl font-bold m-1">Max McDaniel</p>
        <div class="w-0.5 h-4 bg-gray-300 opacity-20 m-1 rounded-xl"></div>
        <p id="email-button" class="text-gray-300 font-xl font-bold m-1 hover:underline underline-offset-2 cursor-pointer">me@dodoseal.com</p>
    </div>

    <!-- Navigation Buttons -->
    <div class="w-75 h-full flex center-content">
        <a href="/" class="{currentRoute === "/" ? "text-gray-300" : "text-gray-500"} font-xl font-bold m-4 hover:text-gray-300 transition-colors duration-200 cursor-pointer" id="nav-home">Home</a>
        <a href="/portfolio" class="{currentRoute === "/portfolio" ? "text-gray-300" : "text-gray-500"} font-xl font-bold m-4 hover:text-gray-300 transition-colors duration-200 cursor-pointer" id="nav-portfolio">Portfolio</a>
        <a href="/contact" class="{currentRoute === "/contact" ? "text-gray-300" : "text-gray-500"} font-xl font-bold m-4 hover:text-gray-300 transition-colors duration-200 cursor-pointer" id="nav-contact">Contact</a>
    </div>
</div>