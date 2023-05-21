<script>
    import { page } from "$app/stores";
    const greetings = {
        en: "Hello",
        zh: "妳好!",
        es: "Hola!",
    };

    const {lang = 'en'}  = $page.params;
    const greeting = greetings[lang] || greetings['zh']
</script>

<h1>{greeting}</h1>
