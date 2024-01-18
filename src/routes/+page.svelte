<script>
    import Intros from "$lib/components/QuickInfoCards/CardSlider.svelte";
    import Introduction from "$lib/components/Introduction.svelte";
    import { fly } from "svelte/transition";
</script>

<div
    in:fly={{ y: 50, duration: 500, delay: 500 }}
    out:fly={{ y: -50, duration: 250 }}
    class="m-0 h-0"
>
    <div
        class="mx-auto my-20 text-center duration-200 ease-in md:my-28 lg:my-36"
    >
        <Introduction></Introduction>
        <Intros></Intros>
    </div>
</div>
