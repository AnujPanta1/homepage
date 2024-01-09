<script>
    import { fade, fly } from "svelte/transition";
    let phraseIndex = 0;
    let phrases = [
        "i'm a cs student at uc berkeley",
        "i've worked @ apple & w/ uc berkeley law",
        "i love to make websites",
        "please check out more :-)",
    ];

    setInterval(() => {
        phraseIndex = phraseIndex + 1 === phrases.length ? 0 : phraseIndex + 1;
    }, 6000);
</script>

<div class="text-center mx-auto translate-y-44">
    <p class="text-3xl font-normal">hi, welcome to my site i'm</p>
    <p class="text-8xl font-bold">Anuj Panta</p>
    <div class="my-5">
        {#each phrases as phrase, i}
            {#if i === phraseIndex}
                <p
                    class="text-4xl font-semibold h-0 m-0"
                    in:fly={{ y: 50, duration: 500, delay: 500 }}
                    out:fade={{ duration: 500 }}
                >
                    {phrase}
                </p>
            {/if}
        {/each}
    </div>
</div>
