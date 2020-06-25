<script>
    export let duration = 1000;

    let loopBool = false;
    setInterval(() => {
        loopBool = !loopBool
    }, duration - 250);

    const float = (node, { duration }) => ({
        duration,
        css: t => `box-shadow: ${t * 8}px ${t * 8}px ${t * 12}px #bbb, ${t * -8}px ${t * -8}px ${t * 12}px #bbb, ${t * 8}px ${t * -8}px ${t * 12}px #bbb, ${t * -8}px ${t * 8}px ${t * 12}px #bbb`
    });
</script>

{#if loopBool}
    <div transition:float={{ duration: duration }} class="my-4 p-4 mx-4 md:w-1/2 md:mx-auto">
        <slot />
    </div>
{/if}