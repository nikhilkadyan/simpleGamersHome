<template>
    <div class="faq_container">
        <h2>
            <i class="fa fa-question-circle text-primary" aria-hidden="true"></i> 
            <span class="text-primar">
                F.A.Q.
            </span>

            {{ fetchedQnA }}
            <div class="card mt-5" v-for="qna in qnas" :key="qna.question">
                <div class="card-body">
                    <h2 class="card-title">
                        {{ qna.question }}
                    </h2>
                    <p class="card-text">
                        {{ qna.answer }}
                    </p>
                </div>
            </div>


        </h2>
    </div>
</template>

<style lang="css" scoped>
    .faq_container{
        min-height: 100vh;

        display: flex;
        justify-content: center;
        align-items: center;
    }
    .card-body > p{
        font-size: 1.1rem;
    }
</style>

<script>
import faqData from '../static/data/faq.json'
export default {
    data() {
        return{
            qnas: faqData
        }
    }
}
</script>