<script>
    import { goto, beforeNavigate, afterNavigate } from "$app/navigation";
    export let productId = 1000;

    beforeNavigate((navigation) => console.log('do this first', {before: navigation}));
    afterNavigate((navigation) => console.log({after: navigation}));
</script>

<a href="/">Home</a>

<h1>product offerings</h1>
<h2>a small duckling</h2>
<h2>two floor tiles</h2>
<h2><a href={`/products/${productId}`}>smattering of {productId} cakes</a></h2>
