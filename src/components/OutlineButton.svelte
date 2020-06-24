<script>
    export let label;
    export let onClick;
</script>

<button class="text-xl p-4 m-4 focus:outline-none border-2 border-black rounded-md active:text-white active:bg-black transition ease-in duration-200" on:click={() => onClick()}>{label}</button>