<script>
    import Intros from "$lib/components/Intros.svelte";
    import Title from "$lib/components/Title.svelte";
    import { fly } from "svelte/transition";
</script>

<div
    in:fly={{ y: 50, duration: 500, delay: 500 }}
    out:fly={{ y: -50, duration: 500 }}
    class="h-0 m-0"
>
    <div class="text-center mx-auto my-20 md:my-40">
        <Title></Title>
        <Intros></Intros>
    </div>
</div>
