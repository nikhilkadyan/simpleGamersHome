<template>
    <div class="faq_container">
        <h2>
            <i class="fa fa-question-circle text-primary" aria-hidden="true"></i> 
            <span class="text-primar">
                F.A.Q.
            </span>

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
export default {
    data() {
        return{
            qnas: [
                {
                    question: 'Is SG Builder Completely Free?',
                    answer:'Yes, SG Builder is completely free and forever will.'
                },
                {
                    question: 'Do SG Builder Take Any Commission?',
                    answer:'No, We Do not Take any Commission. Its 0% Commission 100% Free.'
                },
                {
                    question: 'How Does SG Builder Cover the Server Cost?',
                    answer:'We Run Ads On Our Community as well as on Our Other Websites. We Do Earn From Selling Our Extensions for Other Builders. Our Server Cost is Currently on par with our revenue'
                },
                {
                    question: 'How Often Do We Publish Updates?',
                    answer: 'We Plan on Publishing Patches Per Week and A Major Update Per Month. We take Suggestions from Our Community.'
                }
            ]
        }
    }
}
</script>