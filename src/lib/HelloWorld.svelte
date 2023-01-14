<script>
    let name = "Svelte + Vite";
    let string = "this string contains some <strong>HTML</strong>";
</script>

<p>Hello {name}</p>
<p>{string}</p>
<p>{@html string}</p>

<style>
    p {
        color: reb;
        font-family: "Cascadis Mono";
        font-size: 1em;
    }
</style>
