<script>
    import { fly } from "svelte/transition";
    import LargeWrapper from "$lib/components/LargeWrapper.svelte";
</script>

<div in:fly={{ y: 50, duration: 500, delay: 500 }} class="h-0 m-0">
    <LargeWrapper title="Resume">
        <iframe
            src="anujpantaresume.pdf"
            title="Resume"
            class="w-10/12 mx-auto h-[80%] my-10"
        >
        </iframe>
    </LargeWrapper>
</div>
