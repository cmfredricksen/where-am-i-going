<script lang="ts">

    const links: {
        title: string;
        path: string
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
            title: "Places",
            path: "/places"
        }
    ]

</script>

<nav>
    {#each links as {title, path}}
    <a href={path}>{title}</a>
    {/each}
</nav>

<style>
    nav {
        display: flex;
        justify-content: space-between;
    }

    a {
        margin: 0 1rem;
        text-decoration: none;
    }

    a:hover {
        color: var(--clr-accent);
        font-weight: bold;
    }
</style>