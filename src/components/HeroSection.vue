<template>
  <div class="container-fluid top-117" id="Hero">
     <div class="col-md-12">
         <div class="row">
             <div class="col-md-6 display_flex_align_center">
                 <div class="text-left">
                     <h1 v-if="this.$parent.leneng">Welcome to ArtDev</h1>
                     <h1 v-if="this.$parent.lenfrench">Bienvenus chez ArtDev</h1>
                     <p v-if="this.$parent.leneng" class="fs-18">ArtDev or Artisans Developers Team is a digital solution office, a digital agency
                          in Algeria. ArtDev was founded for modern and fast solutions.
                           we work with clients in different fields of business and services, 
                           medicine, production, logistics, etc. we create the best
                          digital solutions for our friendly customers and the market.</p>

                     <p v-if="this.$parent.lenfrench" class="fs-18">
                        ArtDev est un bureau de solution numérique, une agence numérique en Algérie. 
                        ArtDev a été fondée pour des solutions modernes et rapides. nous travaillons
                        avec des clients dans les domaines , des biens et services , de la médecine, de 
                        la production, de la logistique, etc. nous créons les meilleures solutions digital
                        pour nos aimable clients et le marché.
                        Algeries, 16000, ALGERIA
                       </p>     
                      <button v-if="this.$parent.leneng"
                       class="contact-btn bgc-red"
                        data-toggle="modal" data-target="#contactpreorder">Contact or pre-order</button>    
                       <button v-if="this.$parent.lenfrench" 
                       class="contact-btn bgc-red"
                        data-toggle="modal" data-target="#contactpreorder">Contact ou pré-commande</button>    
                 
                 </div>
             </div>
             <div class="col-md-6 d-none d-md-block ">
                 <img src="images/hherosectionbg.png" class="col">
             </div>
         </div>
     </div>
  </div>
</template>

<script>
export default {
  name: 'HeroSection',
 
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

  .contact-btn{
      border:none;
      padding:15px;
      color:#fff;
      border-radius: 5px;
      cursor: pointer;
  }
</style>
