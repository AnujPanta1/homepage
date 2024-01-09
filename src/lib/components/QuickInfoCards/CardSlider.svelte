<script>
    // @ts-nocheck
    import CardWrapper from "./CardWrapper.svelte";
    import Projects from "./Projects.svelte";
    import Blog from "./Blog.svelte";
    import Resume from "./Resume.svelte";
    import { fade } from "svelte/transition";

    let introIndex = 0;
    let introductions = [
        {
            component: Projects,
            link: "/projects",
        },
        {
            component: Resume,
            link: "/resume",
        },
        {
            component: Blog,
            link: "/blog",
        },
    ];

    function move(n) {
        introIndex += n;

        if (introIndex < 0) {
            introIndex = introductions.length - 1;
        }

        if (introIndex > introductions.length - 1) {
            introIndex = 0;
        }
    }
</script>

<div class="flex my-10 md:my-24 gap-2 px-4 mx-auto w-fit md:gap-5 h-44">
    <button
        on:click={() => {
            move(-1);
        }}
        class="md:hover:scale-125 active:scale-90 duration-150 ease-in"
    >
        <svg
            xmlns="http://www.w3.org/2000/svg"
            class="icon icon-tabler icon-tabler-square-rounded-chevrons-left"
            width="28"
            height="28"
            viewBox="0 0 24 24"
            stroke-width="1.5"
            stroke="#2c3e50"
            fill="none"
            stroke-linecap="round"
            stroke-linejoin="round"
        >
            <path stroke="none" d="M0 0h24v24H0z" fill="none" />
            <path d="M15 15l-3 -3l3 -3" />
            <path d="M11 15l-3 -3l3 -3" />
            <path
                d="M12 3c7.2 0 9 1.8 9 9s-1.8 9 -9 9s-9 -1.8 -9 -9s1.8 -9 9 -9z"
            />
        </svg>
    </button>
    <div>
        {#each introductions as intro, i}
            {#if i === introIndex}
                <div
                    in:fade={{ duration: 400, delay: 300 }}
                    out:fade={{ duration: 200 }}
                    class="m-0 h-0"
                >
                    <a href={intro.link}>
                        <CardWrapper>
                            <svelte:component this={intro.component}
                            ></svelte:component>
                        </CardWrapper>
                    </a>
                </div>
            {/if}
        {/each}
    </div>
    <button
        class="md:hover:scale-125 active:scale-90 duration-150 ease-in"
        on:click={() => {
            move(1);
        }}
    >
        <svg
            xmlns="http://www.w3.org/2000/svg"
            class="icon icon-tabler icon-tabler-square-rounded-chevrons-right"
            width="28"
            height="28"
            viewBox="0 0 24 24"
            stroke-width="1.5"
            stroke="#2c3e50"
            fill="none"
            stroke-linecap="round"
            stroke-linejoin="round"
        >
            <path stroke="none" d="M0 0h24v24H0z" fill="none" />
            <path d="M9 9l3 3l-3 3" />
            <path d="M13 9l3 3l-3 3" />
            <path
                d="M12 3c7.2 0 9 1.8 9 9s-1.8 9 -9 9s-9 -1.8 -9 -9s1.8 -9 9 -9z"
            />
        </svg>
    </button>
</div>
