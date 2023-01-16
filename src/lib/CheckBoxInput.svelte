<script>
    let yes = false;
</script>

<input type="checkbox" bind:checked={yes} />
Yes!Send me regular email spam

{#if yes}
    <p>Thank you, We will bombard your inbox and sell your personal details.</p>
{:else}
    <p>You must opt-in to coninue.If you're not paying, you're the product.</p>
{/if}
