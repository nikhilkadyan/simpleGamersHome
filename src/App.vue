<template>
    <div class="container">
        
        <Landing />
        <div class="margin_top_100"></div>
        <Features />
        <Requirments />
        <Faq />
        <Footer />

    </div>
</template>

<style lang="css">

    .margin_top_100{
        margin-top: 100vh;
    }
    @media only screen and (max-width: 500px){
      .margin_top_100{
          margin-top: calc(100vh - 56px);
      }        
    }
</style>

<script>
import Landing from './components/Landing'
import Features from './components/Features'
import Requirments from './components/Requirments'
import Faq from './components/Faq'
import Footer from './components/Footer'

export default {
    name: 'App',
    components: {
        Landing,
        Features,
        Faq ,
        Requirments,
        Footer,
    }
}
</script>