<script>
    import { slide } from "svelte/transition";
    import Card from "./Card.svelte";

    export let duration = 1000;
    export let title;

    let expanded = false;
    const toggleExpanded = () => expanded = !expanded;
</script>


<Card>
    <div class="flex flex-row justify-between">
        <h1 class="flex-auto text-2xl p-2">{title}</h1>
        <p class="text-3xl p-2 cursor-pointer" on:click={toggleExpanded}>
            {#if expanded}
                x
            {:else}
                +
            {/if}
        </p>
    </div>
    {#if expanded}
        <div transition:slide={{ duration: duration }}>
            <slot />
        </div>
    {/if}
</Card>
