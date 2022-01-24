<script>

    export let items = [
        {
            "name" : "Home",
            "link" : "/"
        },
        {
            "name" : "About",
            "link" : "/about"
        },
        {
            "name" : "FAQ",
            "link" : "/faq"
        },
        {
            "name" : "Press Kit",
            "link" : "/presskit"
        }
    ];
</script>

<ul>
    {#each items as item}
    <li><a href={item.link}>{item.name}</a></li>
    {/each}
</ul>