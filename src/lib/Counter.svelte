<script>
  let count = 0;
  const incre = () => count++;
  $: doubled = count * 2;

  let numbers = [1, 2, 3, 4];
  const addNumber = () => {
    numbers = [...numbers, numbers.length + 1];
  };
  $: sum = numbers.reduce((t, n) => t + n, 0);
</script>

<button on:click={incre}
  >Clicked {count} {count === 1 ? "time" : "times"}
</button>

<p>{doubled}</p>

<p>{numbers.join(" + ")} = {sum}</p>

<button on:click={addNumber}>
	Add a number
</button>