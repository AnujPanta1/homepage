<script>
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
    }, 3300);
</script>

<p class="text-base font-normal md:text-xl lg:text-2xl">
    hi, welcome to my site i'm
</p>
<p class="text-5xl font-bold md:text-7xl lg:text-8xl">Anuj Panta</p>
<div class="my-5 h-10">
    {#each phrases as phrase, i}
        {#if i === phraseIndex}
            <p
                class="text-xl font-semibold md:text-2xl lg:text-3xl"
                in:fly={{ y: 50, duration: 500, delay: 500 }}
                out:fade={{ duration: 300 }}
            >
                {phrase}
            </p>
        {/if}
    {/each}
</div>
