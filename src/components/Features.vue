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
                <span class="text-alternate"> {{ quote.content }} </span>
                <i class="fa fa-quote-right text-primary" aria-hidden="true"></i>

                <br>
                <br>
                <h4 class="text-primary">
                By {{ quote.credit }}

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
import featuresData from '../assets/data/features.json'
import quoteData from '../assets/data/quote.json'
export default {
    data (){
        return{
            features: featuresData,
            quote: quoteData
        }
    }
}
</script>