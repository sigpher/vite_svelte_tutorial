<script>
    import { createEventDispatcher } from "svelte";

    const dispatch = createEventDispatcher();
    const sayHello = () => {
        dispatch("info", {
            text: "svelte demo",
        });
    };
</script>

<button on:click={sayHello}>BTN</button>
