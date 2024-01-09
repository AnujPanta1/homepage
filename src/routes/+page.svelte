<script>
    import Intros from "$lib/components/QuickInfoCards/CardSlider.svelte";
    import Introduction from "$lib/components/Introduction.svelte";
    import { fly } from "svelte/transition";
</script>

<div
    in:fly={{ y: 50, duration: 500, delay: 500 }}
    out:fly={{ y: -50, duration: 250 }}
    class="h-0 m-0"
>
    <div class="text-center mx-auto my-20 md:my-40">
        <Introduction></Introduction>
        <Intros></Intros>
    </div>
</div>
