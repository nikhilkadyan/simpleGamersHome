<template>
    <div class="features_container">
        <h1 class="text-dark text-center">Why Us ?</h1>
        <div class="row">

        <div class="col-12 col-md-4 mt-4 mb-5" v-for="feature in features" :key="feature.name">
            <div class="card_cust">
                <h2>
                    <i v-bind:class="feature.icon"></i>
                    {{ feature.name }}
                </h2>
                <p>
                    {{ feature.content }}
                </p>
            </div>
        </div>
        </div>

        <hr>
        <div class="quote_container">
            <div>
                <i class="fa fa-quote-left text-primary" aria-hidden="true"></i>
                <span class="text-alternate">

                First time I felt like this is my own Builder & Community,
                I have been using other App builders also but when I came across SG,
                its community, the highly capable App Buider and the community made me
                stay here, I am Keeping it. I'm Lovin It.

                </span>
                <i class="fa fa-quote-right text-primary" aria-hidden="true"></i>

                <br>
                <br>
                <h4 class="text-primary">
                By Himanshu

                </h4>
            </div>
        </div>
    </div>
</template>


<style lang="css" scoped>
    .features_container{
        font-family: 'Livvic', sans-serif;
        padding-top: 7vh;
    }
    .card_cust{
        padding: 10% 5%;

        text-align: center;
        max-height: 250px;

        background: white;
        border-radius: 0.625rem;
        box-shadow: 0 2px 6px rgba(0,0,0,.2);
    }
    .card_cust > p{
        font-weight: 100;
        margin-bottom: 0;
    }

    .quote_container{
        height: 90vh;

        display: flex;
        justify-content: center;
        align-items: center;

        text-align: center;
        font-size: 2rem;
    }
    @media only screen and (max-width: 500px) {
        .card_cust > p{
            font-weight: 300;
        }
        .quote_container{
            font-size: 1.3rem
        }
    }
</style>

<script>
export default {
    data (){
        return{
            features: [
                {
                    name: 'Regular Updates',
                    content: 'We Release Patches Per Week and Major Updates Per Month. New Components are Added After Listening to Our Community.',
                    icon: 'fa fa-connectdevelop text-primary'
                },
                {
                    name: 'For the Community',
                    content: 'We Listen To Our Community And Take Suggestions Seriously. New Features Requested In the Community Are Added Into the Builder If Possible.',
                    icon: 'fa fa-comment  text-primary'
                },
                {
                    name: 'Easy & Fast Dev',
                    content: 'Develop Professional Apps In Just Minutes With SG Builder.Its Easy to Understand and Fast For Developement',
                    icon: 'fa fa-clock-o  text-primary'
                },
            ]
        }
    }
}
</script>