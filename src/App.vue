<template>
  <div id="app">
    <LandingPage />
  </div>
</template>

<script>
import LandingPage from './pages/LandingPage.vue'

export default {
  name: 'App',
  components: {
    LandingPage
  }
}
</script>

<style  >


 
   .top-117{
     position:relative;
    top:117px;
   }
   h1,h2,h3,h4,h5,h6 {
      font-family: "quicksand-medium"  !important;
      color:#fff;
      }
      p , span, div,input ,li a{
      font-family: "quicksand-light"  !important;
      color:#fff;
      }
 .text-red{
   color:#cc0a0a;
 }
 .bgc-red{
   background-color:#cc0a0a;
 }
 .text-black{
   color:#161819;
 }
 .bgc-black{
   background-color: #161819;
 }
</style>