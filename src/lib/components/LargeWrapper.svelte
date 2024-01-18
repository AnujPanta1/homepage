<script lang="ts">
    export let title: string;
    export let linkLocation = "/";
    export let color: string;
</script>

<div
    class="w-10/12 md:my-14 bg-white border shadow-sm rounded-xl py-3 bg-white/90 mx-auto h-[85vh] mt-5 overflow-y-scroll"
>
    <div class="flex w-full justify-between items-center border-b px-4 pb-2">
        <p class="font-semibold text-lg">
            <span class={color}>
                {title}
            </span>
        </p>
        <a
            href={linkLocation}
            class="p-1.5 rounded-lg hover:bg-stone-200/80 duration-300 ease-in active:scale-90"
        >
            <svg
                xmlns="http://www.w3.org/2000/svg"
                class="icon icon-tabler icon-tabler-x"
                width="20"
                height="20"
                viewBox="0 0 24 24"
                stroke-width="1.5"
                stroke="#2c3e50"
                fill="none"
                stroke-linecap="round"
                stroke-linejoin="round"
            >
                <path stroke="none" d="M0 0h24v24H0z" fill="none" />
                <path d="M18 6l-12 12" />
                <path d="M6 6l12 12" />
            </svg>
        </a>
    </div>

    <slot />
</div>
