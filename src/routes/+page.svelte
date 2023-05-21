<script>
    import {goto, beforeNavigate, afterNavigate} from '$app/navigation'

    const blogpages = ['animals', 'birthrights','constellations','dinosaurs','evolutions'
]
    const handleClick = () =>{
        console.log('placing your order');
        goto('products', {replaceState: true})
    }
    beforeNavigate(()=> console.log('do this first'))
</script>

<body>
    
    <h1>You've Arrived</h1>
    <ul>
    {#each blogpages as page }
        <li>
            <a href="/blog/{page}">{page} blog</a>
        </li>
    {/each}
    </ul>

    <button on:click={handleClick}>CLICK HERE</button>
</body>

<style>
    body{
        background-color:  rgb(224, 222, 222)
    }
    
</style>