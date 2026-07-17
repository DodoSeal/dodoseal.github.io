<script lang="ts">
    import { page } from "$app/state";
	import Navbar from "$lib/assets/Navbar.svelte";

    const errorCode = page.status;
    const errorMsg = page.error?.message || "An Error Occurred";
</script>

<div class="main-wrapper">
    <Navbar />
    <div class="main-content center-content flex-col">
        <p class="text-gray-300 text-[10rem] font-bold">{errorCode}</p>
        <p class="text-gray-300 text-[5rem] font-bold">{errorMsg}</p>
    </div>
</div>