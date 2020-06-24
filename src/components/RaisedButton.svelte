<script>
    export let label;
    export let onClick;
    export let darkMode = false;
</script>

{#if !darkMode}
    <button class="p-4 m-4 text-xl shadow-md border-2 bg-white active:shadow-none focus:outline-none transition ease-in duration-200 rounded-md" on:click={() => onClick()}>
        {label}
    </button>
{:else}
    <button class="p-4 m-4 text-xl text-white active:text-black shadow-md bg-black active:bg-white focus:outline-none transition ease-in duration-200 rounded-md" on:click={() => onClick()}>
        {label}
    </button>
{/if}