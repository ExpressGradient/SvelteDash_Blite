<script>
    export let label;
    export let onChange;

    let inputValue = "";
    $: onChange(inputValue);
</script>

<label class="block m-4 p-4 text-2xl text-center">
    {label}
    <input value={inputValue} class="block shadow-inner p-2 focus:outline-none border-2 rounded-md w-full text-xl">
</label>