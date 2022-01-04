<script lang="ts">
    import { writable, derived } from "svelte/store";
    const width = writable(0);
    export const isMobile = derived(width, ($width) => $width <= 1440);
</script>

<svelte:window bind:innerWidth={$width} />
