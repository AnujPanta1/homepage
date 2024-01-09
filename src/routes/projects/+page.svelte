<script>
    import { fly } from "svelte/transition";
</script>

<div in:fly={{ y: 50, duration: 500, delay: 500 }} class="h-0 m-0">
    <div
        class="w-8/12 bg-white border shadow-sm rounded-xl py-3 bg-white/90 mx-auto my-10 max-h-[90vh] overflow-y-scroll"
    >
        <div
            class="flex w-full justify-between items-center border-b px-4 py-2"
        >
            <p class="font-semibold text-lg">Projects</p>
            <a
                href="/"
                class="p-1.5 rounded-lg hover:bg-gray-100/80 duration-300 ease-in active:scale-90"
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

        <div class="px-4 py-2">
            <div class="border-b py-3 mb-3">
                <p class="text-xs font-semibold uppercase text-gray-600">
                    Websites
                </p>
                <div class="flex flex-wrap gap-3 my-2">
                    <div
                        class="text-left py-3 px-5 rounded-lg hover:bg-stone-200/80 duration-300 text-sm"
                    >
                        <p class="text-blue-600 font-semibold">
                            Youtube Ripper
                        </p>
                        <p class="text-gray-600 my-2">
                            okay im doing things in youtube rupper again okay
                            yay !
                        </p>
                    </div>
                    <div
                        class="text-left py-3 px-5 rounded-lg hover:bg-stone-200/80 duration-300 text-sm"
                    >
                        <p class="text-blue-600 font-semibold">
                            Youtube Ripper
                        </p>
                        <p class="text-gray-600 my-2">
                            okay im doing things in youtube rupper again okay
                            yay !
                        </p>
                    </div>
                    <div
                        class="text-left py-3 px-5 rounded-lg hover:bg-stone-200/80 duration-300 text-sm"
                    >
                        <p class="text-blue-600 font-semibold">
                            Youtube Ripper
                        </p>
                        <p class="text-gray-600 my-2">
                            okay im doing things in youtube rupper again okay
                            yay !
                        </p>
                    </div>
                    <div
                        class="text-left py-3 px-5 rounded-lg hover:bg-stone-200/80 duration-300 text-sm"
                    >
                        <p class="text-blue-600 font-semibold">
                            Youtube Ripper
                        </p>
                        <p class="text-gray-600 my-2">
                            okay im doing things in youtube rupper again okay
                            yay !
                        </p>
                    </div>
                </div>
            </div>

            <div class="py-3 border-b mb-3">
                <p class="text-xs font-semibold uppercase text-gray-600">
                    Animations
                </p>
                <div class="flex flex-wrap gap-3 my-2">
                    <div
                        class="text-left py-3 px-5 rounded-lg hover:bg-stone-200/80 duration-300 text-sm"
                    >
                        <p class="text-blue-600 font-semibold">
                            Youtube Ripper
                        </p>
                        <p class="text-gray-600 my-2">
                            okay im doing things in youtube rupper again okay
                            yay !
                        </p>
                    </div>
                    <div
                        class="text-left py-3 px-5 rounded-lg hover:bg-stone-200/80 duration-300 text-sm"
                    >
                        <p class="text-blue-600 font-semibold">
                            Youtube Ripper
                        </p>
                        <p class="text-gray-600 my-2">
                            okay im doing things in youtube rupper again okay
                            yay !
                        </p>
                    </div>
                    <div
                        class="text-left py-3 px-5 rounded-lg hover:bg-stone-200/80 duration-300 text-sm"
                    >
                        <p class="text-blue-600 font-semibold">
                            Youtube Ripper
                        </p>
                        <p class="text-gray-600 my-2">
                            okay im doing things in youtube rupper again okay
                            yay !
                        </p>
                    </div>
                    <div
                        class="text-left py-3 px-5 rounded-lg hover:bg-stone-200/80 duration-300 text-sm"
                    >
                        <p class="text-blue-600 font-semibold">
                            Youtube Ripper
                        </p>
                        <p class="text-gray-600 my-2">
                            okay im doing things in youtube rupper again okay
                            yay !
                        </p>
                    </div>
                </div>
            </div>

            <div class="py-3 border-b mb-3">
                <p class="text-xs font-semibold uppercase text-gray-600">
                    Others
                </p>
                <div class="flex flex-wrap gap-3 my-2">
                    <div
                        class="text-left py-3 px-5 rounded-lg hover:bg-stone-200/80 duration-300 text-sm"
                    >
                        <p class="text-blue-600 font-semibold">
                            Youtube Ripper
                        </p>
                        <p class="text-gray-600 my-2">
                            okay im doing things in youtube rupper again okay
                            yay !
                        </p>
                    </div>
                </div>
            </div>
        </div>
        <div class="px-4 mb-2">
            <p class="text-sm mx-auto font-semibold text-gray-600 w-fit">
                Gheck out my saucy github !
            </p>
        </div>
    </div>
</div>

<style>
    p {
        width: fit-content;
    }
</style>
