<script>
    import { page } from "$app/stores";
    const paramlist = $page.params.slug.split("/");
</script>

<h1>Docs homepage</h1>
<h3>all you want for Christmas is:</h3>
<ul>
    {#each paramlist as param}
        <li>
            a {param}
        </li>
    {/each}
</ul>
