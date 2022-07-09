<script lang="ts">
    import "../global.css";
    import Header from "$lib/header.svelte";
    import { toggle } from "../stores/toggle";
    import DropDownMenu from "$lib/components/drop-down-menu.svelte";
    import Footer from "$lib/footer.svelte";

    $toggle = false;
</script>



<Header />

<div class="wrapper">
    {#if $toggle}
    <DropDownMenu />
    {/if}
    <slot />
</div>

<Footer />

<style>
    .wrapper {
        width: 70%;
        margin: 1rem auto;
    }
</style>