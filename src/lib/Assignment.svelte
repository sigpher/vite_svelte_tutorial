<script>
    let count = 0;
    const incre = () => count++;

    $: doubled = count * 2;
</script>

<button on:click={incre}>{count}</button>
<p>{doubled}</p>

<style>
    button {
        border-width: 1px;
        padding: 20px;
        border-radius: 10%;
    }
</style>
