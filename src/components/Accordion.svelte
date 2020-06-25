<script>
    import { slide } from "svelte/transition";
    import Card from "./Card.svelte";

    export let duration = 1000;

    let expanded = false;
    const toggleExpanded = () => expanded = !expanded;
</script>


<Card>
    <div class="flex flex-row justify-between">
        <h1 class="flex-auto text-2xl p-2">Hello World</h1>
        <p class="text-3xl p-2 cursor-pointer" on:click={toggleExpanded}>
            {#if expanded}
                x
            {:else}
                +
            {/if}
        </p>
    </div>
    {#if expanded}
        <p class="text-xl" transition:slide={{ duration: duration }}>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Assumenda commodi corporis eaque enim harum illum ipsa itaque laborum minus nam nobis, nostrum quas quia quisquam recusandae reprehenderit, repudiandae sed sequi veritatis voluptatibus. Adipisci blanditiis fugit illo minima numquam quod temporibus totam. Aliquam dolore doloremque fugiat odit quae repellendus repudiandae similique.</p>
    {/if}
</Card>
