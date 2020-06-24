<script>
    export let label;
    export let onChange;

    let inputValue = "";
    $: onChange(inputValue);
</script>

<label class="text-xl block m-4 md:text-center md:w-1/4">
    {label}
    <input bind:value={inputValue} class="shadow-inner border-2 focus:outline-none p-2 block md:w-full"/>
</label>