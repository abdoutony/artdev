<template>
  <div class="container-fluid top-117 footer-container" id="Contacts">
      <div class="container">
          <hr class="bg-white">

          <div class="row p-t-50">

              <div class="col-md-3 logo-container">
                  <img src="/images/artdevlogofinalwhite.png" alt="logo" width="150">
             </div>
             <div class="col-md-3">
               <div>
                   <p>
                       <i class="fa fa-phone-alt"></i>
                       (+213)657373121
                   </p>
                    <p>
                       <i class="fa fa-phone-alt"></i>
                       (+213)556076810
                   </p>
                    <p>
                       <i class="fa fa-phone-alt"></i>
                       (+213)542354815
                   </p>
               </div>
             </div>
             <div class="col-md-3">
                <p>
                       <i class="fa fa-envelope"></i>
                       contact.artdev@gmail.com
                </p>
             
             </div>

             <div class="col-md-3">
               <span class="socialmedia">
                   <a href="https://facebook.com/Artdevofficial" target="_blank"><i class="fab fa-facebook"></i></a>
               </span>
                <span class="socialmedia">
                  <a href="#"> <i class="fab fa-instagram"></i></a>
               </span>
                <span class="socialmedia">
                   <a href="#"><i class="fab fa-twitter"></i></a>
               </span>
             </div>
          </div>

          <div class="row display_flex_justify_center p-t-50">
              <p v-if="this.$parent.leneng">All right reserved by © ArtDev.2020</p>
              <p v-if="this.$parent.lenfrench">Tous droits reservés par © ArtDev.2020</p>
          </div>
      </div>



      <!-- Modal -->
<div class="modal fade" id="contactpreorder" tabindex="-1" role="dialog" aria-labelledby="exampleModalLabel" aria-hidden="true">
  <div class="modal-dialog modal-dialog-centered" role="document">
    <div class="modal-content bgc-red">
      <div class="modal-header text-center" >
        <h4 class="modal-title  text-center" id="contactpreorderLabel" v-if="this.$parent.leneng">Contact or pre-order</h4>
        <h4 class="modal-title  text-center" id="contactpreorderLabel" v-if="this.$parent.lenfrench">Contact ou pré-commande</h4>
        
        <button type="button" class="close" data-dismiss="modal" aria-label="Close">
          <span aria-hidden="true">&times;</span>
        </button>
      </div>
      <div class="modal-body">
        <p  v-if="this.$parent.lenfrench">
           Si vous voulez en savoir plus sur nous, vous pouvez nous trouver dans nos medias sociaux ou contactez-nous simplement pour plus d'informations ou pour pre-commander un service.
        </p>
        <p  v-if="this.$parent.leneng">
        If you want to know more about us, you can find us in our social media or just contact us for more information or to pre-order
		a service.
        </p>
        <p>
          <span class="socialmedia"><i class="fa fa-envelope"></i></span>
          <span>contact.artdev@gmail.com</span>
        </p>
        <p>
          <span class="socialmedia"><i class="fa fa-phone-alt"></i></span>
          <span>+213(657373121)</span>
          /
          <span>+213(556076810)</span>
          /
          <span>+213(542354815)</span>
        </p>
        <p>
           <span class="socialmedia2">
                   <a href="https://facebook.com/Artdevofficial" target="_blank"><i class="fab fa-facebook"></i></a>
               </span>
                <span class="socialmedia2">
                  <a href="#"> <i class="fab fa-instagram"></i></a>
               </span>
                <span class="socialmedia2">
                   <a href="#"><i class="fab fa-twitter"></i></a>
               </span>
        </p>
      </div>
      <div class="modal-footer">
        <button v-if="this.$parent.leneng" type="button" class="btn btn-dark" data-dismiss="modal">Close</button>
        <button v-if="this.$parent.lenfrench" type="button" class="btn btn-dark" data-dismiss="modal">Fermer</button>
      </div>
    </div>
  </div>
</div>


<!--modal service 1 -->

<div class="modal fade" id="serviceone" tabindex="-1" role="dialog" aria-labelledby="exampleModalLabel" aria-hidden="true">
  <div class="modal-dialog modal-dialog-centered" role="document">
    <div class="modal-content bgc-red">
      <div class="modal-header" >
        <h4 class="modal-title" id="serviceoneLabel" v-if="this.$parent.leneng">Graphic Design</h4>
        <h4 class="modal-title" id="serviceoneLabel" v-if="this.$parent.lenfrench">Design Graphique</h4>
        
        <button type="button" class="close" data-dismiss="modal" aria-label="Close">
          <span aria-hidden="true">&times;</span>
        </button>
      </div>
      <div class="modal-body">
        <p  v-if="this.$parent.lenfrench">
         La conception graphique, création graphique ou aussi graphique design consiste à concevoir, dans le cadre d'une communication visuelle, des supports de communication combinant images, textes ou des video à destination d'un affichage sur écran ou pour une impression pour savoire plus visitez notre page facebook.
        </p>
        <p  v-if="this.$parent.leneng">
       Graphic design, graphic creation , in the context of visual communication, communication media combining images, texts or videos for display on screen or for printing for more information visit our facebook page.
        </p>
        
      </div>
      <div class="modal-footer">
        <button v-if="this.$parent.leneng" type="button" class="btn btn-dark" data-dismiss="modal">Close</button>
        <button v-if="this.$parent.lenfrench" type="button" class="btn btn-dark" data-dismiss="modal">Fermer</button>
      </div>
    </div>
  </div>
</div>

<!-- modal service two -->

<div class="modal fade" id="servicetwo" tabindex="-1" role="dialog" aria-labelledby="exampleModalLabel" aria-hidden="true">
  <div class="modal-dialog modal-dialog-centered" role="document">
    <div class="modal-content bgc-red">
      <div class="modal-header" >
        <h4 class="modal-title" id="servicetwoLabel" v-if="this.$parent.leneng">Creation of websites, mobile & desktop application</h4>
        <h4 class="modal-title" id="servicetwoLabel" v-if="this.$parent.lenfrench">Création des sitesweb , application mobile & desktop</h4>
        
        <button type="button" class="close" data-dismiss="modal" aria-label="Close">
          <span aria-hidden="true">&times;</span>
        </button>
      </div>
      <div class="modal-body">
        <p  v-if="this.$parent.lenfrench">
        Un site web ou une application mobile vous permet d'être connecter sur internet et pour bien marquer sa présence et c'est un meilleur outil pour atteindre vos objectifs. Contrairement aux autres médias et vous pouvez également avoir une application desktop pour gerer vos taches internes pour savoire plus visitez notre page facebook.
        </p>
        <p  v-if="this.$parent.leneng">
        A website or a mobile application allows you to clearly mark your presence and have traffic & audience and it's a better tool to achieve your goals. Unlike other media and you can also have a desktop application to manage your internal tasks for more visit our Facebook page.
        </p>
        
      </div>
      <div class="modal-footer">
        <button v-if="this.$parent.leneng" type="button" class="btn btn-dark" data-dismiss="modal">Close</button>
        <button v-if="this.$parent.lenfrench" type="button" class="btn btn-dark" data-dismiss="modal">Fermer</button>
      </div>
    </div>
  </div>
</div>


<!-- modal service three -->

<div class="modal fade" id="servicethree" tabindex="-1" role="dialog" aria-labelledby="exampleModalLabel" aria-hidden="true">
  <div class="modal-dialog modal-dialog-centered" role="document">
    <div class="modal-content bgc-red">
      <div class="modal-header">
        <h4 class="modal-title" id="servicethreeLabel" v-if="this.$parent.lenfrench">Administration Systèmes</h4>
        <h4 class="modal-title" id="servicethreeLabel" v-if="this.$parent.leneng">Systems Administration</h4>
        
        <button type="button" class="close" data-dismiss="modal" aria-label="Close">
          <span aria-hidden="true">&times;</span>
        </button>
      </div>
      <div class="modal-body">
        <p  v-if="this.$parent.lenfrench">
       Vous avez un problème d'installation d'un logiciel,système ou une gestion d'un grand site profiter de nos service comme gestion des system hébergement ou bien installation et configuration pour savoire plus visitez notre page facebook.
        </p>
        <p  v-if="this.$parent.leneng">
        You have a problem installing a software, system or managing a large site take advantage of our services such as hosting system management or installation and configuration for more visit our facebook page.
        </p>
        
      </div>
      <div class="modal-footer">
        <button v-if="this.$parent.leneng" type="button" class="btn btn-dark" data-dismiss="modal">Close</button>
        <button v-if="this.$parent.lenfrench" type="button" class="btn btn-dark" data-dismiss="modal">Fermer</button>
      </div>
    </div>
  </div>
</div>


<!-- modal service four -->
<div class="modal fade" id="servicefour" tabindex="-1" role="dialog" aria-labelledby="exampleModalLabel" aria-hidden="true">
  <div class="modal-dialog modal-dialog-centered" role="document">
    <div class="modal-content bgc-red">
      <div class="modal-header">
        <h4 class="modal-title" id="servicefourLabel" v-if="this.$parent.leneng">Advertising And SEO</h4>
        <h4 class="modal-title" id="servicefourLabel" v-if="this.$parent.lenfrench">Publicités Et Référencement</h4>
        
        <button type="button" class="close" data-dismiss="modal" aria-label="Close">
          <span aria-hidden="true">&times;</span>
        </button>
      </div>
      <div class="modal-body">
        <p  v-if="this.$parent.lenfrench">
        Le référencement et la publicité ils ont pour objectif d’augmenter la visibilité de votre site sur les moteurs de recherche, toucher un plus grand nombre de visiteurs en utilisant des technique de référencement ou bien avec les réseaux sociaux qui on pour but de faire un marketing digital sur votre entreprise , mark ,produits ,services avec des stratégies de marketing pour savoire plus visitez notre page facebook.
        </p>
        <p  v-if="this.$parent.leneng">
       SEO and advertising they aim to increase the visibility of your site on search engines, reach more visitors using technical SEO or with social networks which aim to do digital marketing on your business, mark, products, services with marketing strategies to know more visit our facebook page.
        </p>
        
      </div>
      <div class="modal-footer">
        <button v-if="this.$parent.leneng" type="button" class="btn btn-dark" data-dismiss="modal">Close</button>
        <button v-if="this.$parent.lenfrench" type="button" class="btn btn-dark" data-dismiss="modal">Fermer</button>
      </div>
    </div>
  </div>
</div>
     
  </div>
</template>

<script>
export default {
  name: 'Footer',
 
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.modal{
  z-index: 99999999;
}
.footer-container{
    padding-top: 80px;
    padding-bottom: 20px;
}
.socialmedia{
    margin-left: 15px;
    margin-right: 15px;
}

.socialmedia a{
    font-size: 22px;
    color: #fff;
    transition-duration: .25s;
}
.socialmedia a:hover{
    color: #CC0A0A;
}


.socialmedia2{
    margin-left: 15px;
    margin-right: 15px;
}

.socialmedia2 a{
    font-size: 22px;
    color: #fff;
    transition-duration: .25s;
}
.socialmedia2 a:hover{
    color: #161819;
}
</style>
