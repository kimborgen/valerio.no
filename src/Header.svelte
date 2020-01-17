<script>
    let header_src = "./images/header.jpg"
</script>

<style>

    :global(body) {
        padding: 0;
        margin: 0;
    }

    
    
    #header {
        width: 100vw;
        position: relative;
    }

    #img {
        width: 100vw;
        transform: translateY(-20vh);
        margin-bottom: -20vh;
        z-index: -1;
    }

    #name {
        margin-top: -30vh;
        position: absolute;
        width: 70vw;
        left: 15vw;
        
        display: flex;
        align-items: center;
        justify-content: center;

        z-index: 100;
        height: 14vh;

        text-align: center;
    }
    
    #name > h1 {
        font-size: 8em;
        color: white;
        text-shadow: -0.3em 0 black, 0 0.3em #222222, 0.3em 0 black, 0 -0.3em #0000FF;
    }


</style>

<div id="header">
    <img  src={header_src} alt="valerio and his intentions" id="img"/>
    <div id="name">
        <h1>Valerio & His Intentions</h1>
    </div>
</div>

