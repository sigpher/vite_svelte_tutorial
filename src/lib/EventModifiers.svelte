<script>
    const handleClick = () => alert("No more alerts");
</script>

<button on:click|once={handleClick}>Click me</button>
