<script>
    import { count } from "./store";
    const decre = () => {
        count.update((n) => n - 1);
    };
</script>

<button on:click={decre}>-</button>
