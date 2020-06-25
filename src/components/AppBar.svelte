<script>
    import Link from "./Link.svelte";
    export let title;
    export let navLinks;
</script>

<div class="m-4 p-4 rounded-md shadow-md border-2 text-center">
    <h1 class="text-4xl cursor-pointer" on:click>{title}</h1>
    <nav class="m-4">
        {#each navLinks as navLink}
            <Link link={{ label: navLink.label, route: navLink.route }}/>
        {/each}
    </nav>
</div>