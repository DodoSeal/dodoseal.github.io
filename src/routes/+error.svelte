<script lang="ts">
    import { page } from "$app/state";
	import Navbar from "$lib/assets/Navbar.svelte";

    const errorCode = page.status;
    const errorMsg = page.error?.message || "An Error Occurred";
</script>

<div class="main-wrapper">
    <Navbar />
    <div class="main-content center-content flex-col">
        <p class="text-red-400 text-[5rem] font-bold">{errorCode}</p>
        <p class="text-red-400 text-[2.5rem] font-bold">{errorMsg}</p>
        <a class="p-4 mt-8 rounded-2xl w-48 h-18 center-content cursor-pointer text-text-light text-xl text-center font-bold bg-gray-800 hover:bg-gray-700 transition-all duration-200" href="/">Return Home</a>
    </div>
</div>