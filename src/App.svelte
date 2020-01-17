<script>
    import Header from './Header.svelte'; 
    import Events from './Events.svelte';
    import About from './About.svelte';
    import Youtube from './Youtube.svelte';
</script>


<style>
    #main {
        width: 100vw;
        display: grid;
        grid-template-columns: 1fr 1fr 1fr 1fr 1fr; 
        grid-auto-flow: row;
        align-items: center;
        align-content: center;
        justify-content:center;
        margin-bottom: 5vw;
    }

    .header {
        grid-column: 1/6;
    }

    .events {
        grid-column: 1/6;
        
    }

    .about {
        grid-column: 1/6;
    }
    
    .youtube {
        grid-column: 1/6;
    }

</style>


<div id="main">
    <div class="header">
        <Header  />
    </div>
    <div class="events">
        <Events  /> 
    </div>

    <div class="about">
        <About />
    </div>

    <div class="youtube">
        <Youtube />
    </div>
</div>
