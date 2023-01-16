<script>
    import { createEventDispatcher } from "svelte";

    const dispatch = createEventDispatcher();

    const sayHello = () => {
        dispatch("info", {
            content: "蔡伟源",
        });
    };
</script>

<button on:click={sayHello}>Click to say hi!</button>
