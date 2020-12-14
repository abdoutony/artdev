<template>
 <div class="container-fluid app_container">
   <NavBar />
  <HeroSection />
  <HowItWorks />
  <OurServices />
  <Portfolio />
  <Footer />
 </div>
</template>

<script>
import NavBar from "../components/NavBar";
import HeroSection from "../components/HeroSection";
import HowItWorks from "../components/HowItWorks";
import OurServices from "../components/OurServices";
import Portfolio from "../components/Portfolio";
import Footer from "../components/Footer";
export default {
  name: 'LandingPage',

  components:{NavBar , HeroSection, HowItWorks , OurServices,Portfolio,Footer},
  data(){
    return{
      leneng:true,
      lenfrench:false
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.app_container{
  padding:0;
}
</style>
