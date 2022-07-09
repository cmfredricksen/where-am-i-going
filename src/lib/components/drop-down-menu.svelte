<script lang="ts">

    const links: {
        title: string;
        path: string;
    }[] = [
        {
            title: "Boston",
            path: "/places/boston"
        },
        {
            title: "Chicago",
            path: "/places/chicago"
        },
        {
            title: "Minneapolis",
            path: "/places/minneapolis"
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
        align-items: flex-end;
    }
    a {
        padding: 1rem 2rem;
        background: #222;
        border: 1px solid #aaa;
        border-radius: .5rem;
        text-decoration: none;
    }
    a:hover {
        color: var(--clr-accent);
        font-weight: bold;
    }
</style>