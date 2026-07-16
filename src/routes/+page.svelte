<script lang="ts">
	import Navbar from "$lib/assets/Navbar.svelte";
	import { onMount } from "svelte";
    let sitePath: string = $state("");

    onMount(() => {
        sitePath = window.location.pathname;
    });
</script>

<div class="main-content center-content flex-col bg-backdrop">
    <Navbar />
</div>