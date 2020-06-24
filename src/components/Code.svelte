<script>
    export let codes;
</script>

<div class="m-4 p-4 rounded-md text-md text-green-400 bg-black font-mono md:w-2/3">
    {#each codes as code}
        <h3>{code}</h3>
    {/each}
</div>