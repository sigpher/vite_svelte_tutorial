<script>
    import { count } from "./store";

    const incre = () => count.update((n) => n + 1);
</script>

<button on:click={incre}>+</button>
