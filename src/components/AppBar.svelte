<script>
    export let title;
</script>

<div class="m-4 p-4 rounded-md shadow-md border-2 text-center">
    <h1 class="text-4xl cursor-pointer" on:click={() => title.onClick()}>{title.label}</h1>
    <nav class="m-4">

    </nav>
</div>