<script>
    const getRandomNumber = async () => {
        const res = await fetch("https://svelte.dev/tutorial/random-number");
        const text = await res.text();
        if (res.ok) {
            return text;
        } else {
            throw new Error(text);
        }
    };
    let promise = getRandomNumber();
    const handleClick = () => (promise = getRandomNumber());
</script>

<button on:click={handleClick}> Get Number </button>

{#await promise}
    <p>...waiting</p>
{:then text}
    <p>{text}</p>
{:catch error}
    <p style="color:red">{error.message}</p>
{/await}
