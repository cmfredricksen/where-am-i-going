<script lang="ts">

    const links: {
        title: string;
        path: string;
    }[] = [
        {
            title: "Home",
            path: "/"
        },
        {
            title: "About",
            path: "/about"
        },
        {
            title: "Chicago",
            path: "/chicago"
        },
        {
            title: "Minneapolis",
            path: "/minneapolis"
        },
        {
            title: "Boston",
            path: "/boston"
        }
    ]
</script>

<div class="drop-down-menu">
    {#each links as link}
    <a href={link.path}>{link.title}</a>   
    {/each}
</div>

<style>
    .drop-down-menu {
        display: flex;
        flex-direction: column;
    }
</style>