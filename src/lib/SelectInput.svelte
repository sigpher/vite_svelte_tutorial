<script>
    let count = [1, 2, 3, 4];
    let selected;
</script>

<select bind:value={selected}>
    {#each count as number}
        <option value={number}>{number}</option>
    {/each}
</select>

<p>{selected}</p>