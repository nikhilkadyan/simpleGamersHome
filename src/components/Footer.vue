<template>
    <div class="footer_container">
        <div>
            <h3>
                <i class="fa fa-info-circle text-primary" aria-hidden="true"></i>
                For More Info Visit Our Community Page
            </h3>

            <a target="_blank" href="https://community.simplegamers.co/" class="btn btn-large btn-primary">
                <i class="fa fa-users" aria-hidden="true"></i> Community
            </a>

            <p class="mt-2">
                <a href="http://appybuilder.com/" target="_blank">
                    Credits to Appy Builder For Source Code Of App Builder
                </a>
            </p>

            <hr>
            <p class="me_credit">
                Website Designed & Maintained by 
                <a href="https://www.nikhilkadyan.com" target="_blank">
                    Nikhil Kadyan.
                </a>
            </p>
        </div>
    </div>
</template>

<style lang="css" scoped>
    .footer_container{
        height: 30vh;
        display: flex;
        justify-content: center;
        align-items: center;
        text-align: center;
    }
    .footer_container > div > .me_credit{
        font-size: 0.8rem;
        margin-top: 1vh;
        margin-bottom: 0vh;
    }
</style>