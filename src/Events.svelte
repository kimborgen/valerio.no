<script>
    import Event from './Event.svelte';
    
    const events = [
        {
            date: "18-02-20", 
            city: "Trondheim",
            venue: "Trondheim calling",
            link: "https://vg.no",
            tickets: "https://tek.no"  
        },

        {
            date: "18-02-20", 
            city: "Trondheim",
            venue: "Trondheim calling",
            tickets: "https://tek.no"  
        },
        {
            date: "18-02-20", 
            city: "Trondheim",
            venue: "Trondheim calling",
            link: "https://vg.no",
        }
    ]



</script>

<style>

/*


        -webkit-box-shadow: 8px 8px 24px -4px rgba(0,0,0,0.44);
        -moz-box-shadow: 8px 8px 24px -4px rgba(0,0,0,0.44);
        box-shadow: 8px 8px 24px -4px rgba(0,0,0,0.44);

*/
    .container {
        width: 100%;
        display: grid;
        grid-template-columns: 1fr 3fr 1fr;
        background-color: #fffdf2;
        margin-top: -1vh;
    }
    
    .events {
        grid-column: 2/3;
        padding: 5vw;
        padding-top:15vh;
        padding-bottom: 15vh;
    }

    h1 {
        display: inline;
        font-size: 4em;
    }

    .content {
        display: grid;
        grid-template-columns: 1fr 1fr 2fr 1fr 1fr;
        align-items: center;
        justify-content: center;
        padding-top: 1vh;
     }


</style>

<div class="container">
    <div class="events">
        <h1>Events</h1>

        <div class="content">
            <h2>Date</h2>
            <h2>City</h2>
            <h2>Venue</h2>
            <h2>Link</h2>
            <h2>Tickets</h2>


            <Event {...events[0]} />
            <Event {...events[1]} />
            <Event {...events[2]} />

        </div>
    </div>
</div>
        


