<script>
    let user = { loggedIn: false };
    const toggle = () => {
        user.loggedIn = !user.loggedIn;
    };
</script>

{#if user.loggedIn}
    <button on:click={toggle}> Log out </button>
{:else}
    <button on:click={toggle}> Log In </button>
{/if}
