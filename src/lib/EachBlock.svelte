<script>
    let persons = [
        { id: 1, name: "choi" },
        { id: 2, name: "lory" },
        { id: 3, name: "tory" },
    ];
</script>

{#each persons as { id, name } (id)}
    <ul>
        <li>{id}:{name}</li>
    </ul>
{/each}

<style>
    ul {
        list-style: none;
    }
    ul:hover {
        background-color: #000;
        color: #fff;
    }
</style>
