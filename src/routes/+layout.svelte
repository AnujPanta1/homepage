<script>
    import { onMount } from "svelte";
    import "../app.pcss";
    // @ts-ignore
    let isChromium = false;
    onMount(() => {
        if (window) {
            // @ts-ignore
            isChromium = !!window.chrome;
        }
    });
</script>

{#if isChromium}
    <p
        class=" text-center font-medium text-gray-300 w-fit mx-auto translate-y-9 md:translate-y-32"
    >
        chrome isn't a fan of animations, open in safari for a better experience
        !
    </p>
{/if}

<slot />
