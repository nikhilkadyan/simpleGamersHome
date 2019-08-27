<template>
    <div class="landing">

        <!-- Landing Content -->
        <div class="landing_content">
            <div>
                <h1>SG Builder</h1>
                <h4>A BUILDER MADE FOR THE COMMUNITY</h4>


                <div class="links">
                    <a target="_blank" href="http://builder.simplegamers.co/" class="mb-2 btn btn-danger">
                        <i class="fa fa-plus-circle" aria-hidden="true"></i> Create App
                    </a>
                    <br>
                    <a target="_blank" href="https://community.simplegamers.co/" class="mr-1 btn btn-dark">
                        <i class="fa fa-users" aria-hidden="true"></i> Community
                    </a>
                    <a target="_blank" href="https://store.simplegamers.co/" class="btn btn-dark">
                        <i class="fa fa-shopping-cart" aria-hidden="true"></i> Store
                    </a>
                </div>
            </div>
        </div>

        <!-- SVG Items -->
        <div id="mobile_svg_container">
            <img src="../assets/images/mobile.svg" id="mobile_svg">
        </div>

    </div>
</template>

<style lang="css">

    .landing{
        height: 100vh;
        width: 100%;
        margin: 0;
        padding: 0;

        position: absolute;
        top: 0;
        left: 0;

        background: url('../assets/images/cg_bg.svg') no-repeat;
        background-size: cover;
        color: white;
        font-family: 'Livvic', sans-serif;

    }
    .landing_content > div{
        height: 70vh;
        padding-top: 30vh;
        padding-left: 5%;
    }
    h1{
        text-transform: uppercase;
        color: white;
        font-size: 3rem;
    }
    #mobile_svg{
        position: absolute;
        top: 25vh;
        right: 0;
        height: 75vh;
    }

    @media only  screen and (max-width: 500px){
        .landing{
            background: linear-gradient(to bottom,#6371d1 30%,#3949abff);
            background-size: cover;
            height: calc(100vh - 56px);
        }
        .landing_content > div{
            height: 70vh;
            padding-top: 10vh;
            padding-left: 2%;
        }
        #mobile_svg{
            height: 40vh;
            right: 0;
            top: calc(60vh - 56px);
        }
    }
</style>