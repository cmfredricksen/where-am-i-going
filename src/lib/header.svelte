<script lang="ts">
    import Nav from "./nav.svelte";
</script>

<header>
<div class="header-title">
    <h1>Where Am I Going?</h1>
    <h3>Making Content From My Dilemma</h3>
</div>

    <Nav />
</header>

<style>
    header {
        display: flex;
        justify-content: space-between;
        align-items: baseline;
        padding: 1rem;
        /* border-bottom: 2px solid var(--clr-white); */
        box-shadow: 5px 5px 5px #000;
    }

    .header-title {
        display: flex;
        align-items: baseline;
    }
    h3 {
        margin: 0 .5rem;
    }
</style>