<script lang="ts">
    interface PageTitle {
        title: string,
        description: string
    };

    const data: PageTitle = $props();
</script>

<div class="w-full pt-16 pb-16 flex flex-col text-text-light gap-y-4">
    <p class="font-bold text-4xl">{data.title}</p>
    <p class="font-bold text-lg text-text-dark">{data.description}</p>
</div>