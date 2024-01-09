<script>
    import { fade } from "svelte/transition";
    export let showDialog = false;
</script>

{#if showDialog}
    <dialog
        open
        transition:fade
        class="absolute top-0 transform overflow-hidden rounded-lg bg-white text-left shadow-xl transition-all sm:my-8 sm:w-full sm:max-w-lg"
    >
        <slot />
    </dialog>
{/if}
