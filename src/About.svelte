<script>
   const about_content = ["Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam", "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum."] 

</script>

<style>
    
    .container {
        background-color: #fffdf2;
        display: grid;
        grid-template-columns: 1fr 2fr;
        grid-flow: column;
        align-items: center;
        justify-content: center;
        padding-left: 5vw;
        padding-right: 5vw;
        padding-bottom: 10vh;
        grid-gap: 5vw;
    }

    .iframe {
        
        height: 40vh;
        width: 100%;
        justify-self: center;
        align-self: center;
        -webkit-box-shadow: 8px 8px 24px -4px rgba(0,0,0,0.44);
        -moz-box-shadow: 8px 8px 24px -4px rgba(0,0,0,0.44);
        box-shadow: 8px 8px 24px -4px rgba(0,0,0,0.44);
    }
    .about {
        height: 28vh;
        padding-top: 6vh;
        padding-bottom: 6vh;
        padding-right: 10vh;
        padding-left: 10vh;
        background-color: #222222;
        color: white;
        display: flex;
        flex-flow: column;
        
        align-content: center;
        -webkit-box-shadow: 8px 8px 24px -4px rgba(0,0,0,0.44);
        -moz-box-shadow: 8px 8px 24px -4px rgba(0,0,0,0.44);
        box-shadow: 8px 8px 24px -4px rgba(0,0,0,0.44);
    }


    .about > p {
        text-align: justify;
    }
    


</style>

<div class="container">
    <div class="iframe">
        <iframe src="https://open.spotify.com/embed/artist/3NzxlaOfBp6IB8b9y6w94j" width="100%" height="100%" frameborder="0" allowtransparency="true" allow="encrypted-media"></iframe>
    </div>
    <div class="about">
        <h1>About</h1>
        {#each about_content as par}
            <p>{par}</p>
        {/each}
    </div>
</div>

