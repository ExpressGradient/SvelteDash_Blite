<script>
    export let label;
    export let onSubmit;
</script>

<form class="m-4 p-4 rounded-md shadow-xl md:w-2/3 border-2" on:submit|preventDefault={onSubmit}>
    <h2 class="text-3xl text-center underline">{label}</h2>
    <slot></slot>
</form>