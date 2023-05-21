<script>
    import { page } from "$app/stores";
    const productId = $page.params.productId;
    const productColor = $page.params.productColor;
</script>

<h1>product details #{productId}</h1>
<h3 style="color:{productColor}">
    in the most fashionable color available: {productColor}
</h3>
