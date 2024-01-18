<script lang="ts">
    export let title: string;
    export let mainText: string;
    export let tags: any;
    export let projectLink: string;
    export let githubLink: string;
</script>

<div
    class="flex flex-col gap-2 rounded-lg px-5 py-3 text-left text-sm duration-300 hover:bg-stone-100/80"
>
    <div>
        <div class="flex items-center justify-between">
            <p class="font-semibold text-blue-600">{title}</p>
            <div
                class=" hover:bg-stone/80 my-0.5 flex gap-2 rounded-lg py-1 duration-100"
            >
                <a
                    href={projectLink}
                    target="_blank"
                    class=" text-black duration-100 hover:text-blue-600/80"
                >
                    <svg
                        xmlns="http://www.w3.org/2000/svg"
                        class="icon icon-tabler icon-tabler-external-link"
                        width="16"
                        height="16"
                        viewBox="0 0 24 24"
                        stroke-width="1.5"
                        stroke="currentColor"
                        fill="none"
                        stroke-linecap="round"
                        stroke-linejoin="round"
                    >
                        <path stroke="none" d="M0 0h24v24H0z" fill="none" />
                        <path
                            d="M12 6h-6a2 2 0 0 0 -2 2v10a2 2 0 0 0 2 2h10a2 2 0 0 0 2 -2v-6"
                        />
                        <path d="M11 13l9 -9" />
                        <path d="M15 4h5v5" />
                    </svg>
                </a>

                <a
                    href={githubLink}
                    target="_blank"
                    class=" text-black duration-100 hover:text-blue-600/80"
                >
                    <svg
                        xmlns="http://www.w3.org/2000/svg"
                        class="icon icon-tabler icon-tabler-brand-github"
                        width="16"
                        height="16"
                        viewBox="0 0 24 24"
                        stroke-width="1.5"
                        stroke="currentColor"
                        fill="none"
                        stroke-linecap="round"
                        stroke-linejoin="round"
                    >
                        <path stroke="none" d="M0 0h24v24H0z" fill="none" />
                        <path
                            d="M9 19c-4.3 1.4 -4.3 -2.5 -6 -3m12 5v-3.5c0 -1 .1 -1.4 -.5 -2c2.8 -.3 5.5 -1.4 5.5 -6a4.6 4.6 0 0 0 -1.3 -3.2a4.2 4.2 0 0 0 -.1 -3.2s-1.1 -.3 -3.5 1.3a12.3 12.3 0 0 0 -6.2 0c-2.4 -1.6 -3.5 -1.3 -3.5 -1.3a4.2 4.2 0 0 0 -.1 3.2a4.6 4.6 0 0 0 -1.3 3.2c0 4.6 2.7 5.7 5.5 6c-.6 .6 -.6 1.2 -.5 2v3.5"
                        />
                    </svg>
                </a>
            </div>
        </div>
        <p class="my-2 text-gray-600">
            {mainText}
        </p>
    </div>

    <div class="flex flex-wrap gap-2">
        {#each tags as tag}
            <span
                class="inline-flex items-center gap-x-1 rounded-full bg-blue-100/80 px-3 py-1 text-xs font-medium text-blue-800/80"
                >{tag}</span
            >
        {/each}
    </div>
</div>
