<script lang="ts">
    import "../global.css";
    import Header from "$lib/header.svelte";
    import { toggle } from "../stores/toggle";
    import DropDownMenu from "$lib/components/drop-down-menu.svelte";
    import Footer from "$lib/footer.svelte";

    $toggle = false;
</script>



<Header />

{#if $toggle}
<DropDownMenu />
{/if}
<button on:click={() => toggle.set(!$toggle)}>&HorizontalLine;</button>
<slot />

<Footer />