<script>
    import CustomButton from "./CustomButton.svelte";
    const handleClick = () => {
        alert("Button Clicked");
    };
</script>

<CustomButton on:click/>
