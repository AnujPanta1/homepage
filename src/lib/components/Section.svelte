<script>
    export let title = "";
</script>

<div class="border-b py-3 mb-3">
    <p class="text-xs font-semibold uppercase text-gray-600">{title}</p>
    <slot />
</div>
