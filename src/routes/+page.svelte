<script>
    import Card from "$lib/components/Card.svelte";
    import Intros from "$lib/components/Intros.svelte";
    import { fade, fly } from "svelte/transition";
    let phraseIndex = 0;
    let phrases = [
        "i'm a cs student at uc berkeley",
        "i've worked on WebKit @ Apple",
        "i love the creative side of code",
        "please check out more :-)",
    ];

    setInterval(() => {
        phraseIndex = phraseIndex + 1 === phrases.length ? 0 : phraseIndex + 1;
    }, 6000);
</script>

<div class="text-center mx-auto translate-y-20 md:translate-y-44">
    <p class="text-lg md:text-3xl font-normal">hi, welcome to my site i'm</p>
    <p class="text-5xl md:text-8xl font-bold">Anuj Panta</p>
    <div class="my-5 h-10 md:h-20">
        {#each phrases as phrase, i}
            {#if i === phraseIndex}
                <p
                    class="text-xl md:text-4xl font-semibold"
                    in:fly={{ y: 50, duration: 500, delay: 900 }}
                    out:fade={{ duration: 1000 }}
                >
                    {phrase}
                </p>
            {/if}
        {/each}
    </div>
    <Intros></Intros>
</div>
