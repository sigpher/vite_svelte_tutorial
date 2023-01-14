<script>
    let numbers = [1, 2, 3, 4];
    const addNumber = () => (numbers = [...numbers, numbers.length + 1]);
    $: sum = numbers.reduce((t, n) => t + n, 0);
</script>

<button on:click={addNumber}>Add Number</button>

<p>{numbers.join(" + ")} = {sum}</p>
