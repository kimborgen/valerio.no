<script>
    export let date; 
    export let city;
    export let venue;

    export let link = false; 
    export let tickets = false;
</script>

<style>
    
    .event {
        width: 100%;
    }

    h1 {
        display: inline;
        font-size: 2em;
    }

    button {
        width: 80%;
        margin-top: 6%;
    }

</style>

<p>{date}</p>
<p>{city}</p>
<p>{venue}</p>
{#if link !== false}
    <a href={link}><button>Arrangement</button></a>
{:else}
    <p></p>
{/if}
{#if tickets !== false}
    <a href={tickets}><button onclick={tickets}>Tickets</button></a>
{:else}
    <p></p>
{/if}


