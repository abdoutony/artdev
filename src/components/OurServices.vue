<template>
  <div class="container-fluid top-117" id="OurServices">
     <div class="col-md-12">
         <div class="row display_flex_justify_center p-t-80">
    
           <div class="text-center">
               <h1 v-if="this.$parent.leneng">Our Services</h1>
                <h1 v-if="this.$parent.lenfrench">Nos Services</h1>
           </div>

         </div>


<div class="row display_flex_justify_center cont p-t-50 ">
<div class="box m-b-15">
<img src="images/graphicdesignimage.png">
<h2>01</h2>
<h3 v-if="this.$parent.leneng">Graphic Design</h3>
<h3 v-if="this.$parent.lenfrench">Conception Graphique</h3>
<p v-if="this.$parent.leneng">logo | flyers | business card | social media design | ads Banner | video editing | website and application tester........</p>
<p v-if="this.$parent.lenfrench"> logo | flyers | carte visite | social media design  | Bannière publicitaire | vidéo editing | website and application tester........</p>

<button v-if="this.$parent.leneng"
 class="bgc-red"
  data-toggle="modal" data-target="#serviceone">Learn More</button>
<button v-if="this.$parent.lenfrench" 
class="bgc-red"
 data-toggle="modal" data-target="#serviceone">Savoir plus</button>
</div>

<div class="box m-b-15">
<img src="images/webdevimages.png">
<h2>02</h2>
<h3 v-if="this.$parent.leneng">Creation of websites, mobile & desktop application</h3>
<h3 v-if="this.$parent.lenfrench">Création des sitesweb , application mobile & desktop</h3>
<p v-if="this.$parent.leneng">
websites : dynamique | static |with single page |showcase |catalogue |entreprise |e-commerce...... application : mobile hybride | app for desktop....... 
</p>
<p v-if="this.$parent.lenfrench">
sitewebs :  dynamique | static |avec une seule page |vitrine |catalogue |entreprise |e-commerce...application : mobile hybride | app pour desktop....... 
</p>
<button v-if="this.$parent.leneng" class="bgc-red"
 data-toggle="modal" data-target="#servicetwo">Learn More</button>
<button v-if="this.$parent.lenfrench"
 class="bgc-red"
 data-toggle="modal" data-target="#servicetwo">Savoir plus</button>
</div>

<div class="box m-b-15">
<img src="images/sysadmin.png">
<h2>03</h2>
<h3 v-if="this.$parent.leneng">Systems Administration</h3>
<h3 v-if="this.$parent.lenfrench">Administration Systèmes</h3>

<p v-if="this.$parent.leneng">
administration of : data base | websites | installation and configuration of softwares and systems...... 
</p>
<p v-if="this.$parent.lenfrench">administration de : base de données | siteweb | installation et configuration des logiciel et système... 
</p>
<button v-if="this.$parent.leneng"
 class="bgc-red" 
  data-toggle="modal" data-target="#servicethree">Learn More</button>
<button v-if="this.$parent.lenfrench" class="bgc-red"
 data-toggle="modal" data-target="#servicethree">Savoir plus</button>
</div>

<div class="box m-b-15">
<img src="images/seo.png">
<h2>04</h2>
<h3 v-if="this.$parent.leneng">Advertising And SEO</h3>
<h3 v-if="this.$parent.lenfrench">Publicité Et Référencement</h3>
<p v-if="this.$parent.leneng">seo | advertising and social media management | increase number of website traffic & visitors | website ranking......</p>
<p v-if="this.$parent.lenfrench">référencement | publicité et gestion des réseaux sociaux | augmentation nombre de visiteurs de siteweb | seo......</p>
<button  v-if="this.$parent.leneng" class="bgc-red"
 data-toggle="modal" data-target="#servicefour">Learn More</button>
<button  v-if="this.$parent.lenfrench" class="bgc-red"
 data-toggle="modal" data-target="#servicefour">Savoir plus</button>
</div>
</div>



     </div>
  </div>
</template>

<script>
export default {
  name: 'OurServices',
 
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>


 .cont 
    {
        display: flex;
        
        justify-content: center;
        flex-wrap: wrap;
    }
    .cont .box
    {
        position: relative;
        width: 280px;
        background: #232425;
        padding: 100px 40px 60px;
        /*box-shadow: 0 15px 45px rgba(0,0,0,.1);*/
        
    }
    .cont .box:nth-child(1),.cont .box:nth-child(2),.cont .box:nth-child(3){
        border-right:8px solid #161819;
    }

    .cont .box:before
    {
        content:''; 
        position: absolute;
        top:0; 
        left:0;     
        width:100%;
        height:100%; 

        background: #cc0a0a/*ff226d*/;
        transform: scaleY(0);
        transform-origin:top; 
        transition: transform 0.5s;
    
    }
     .cont .box:hover:before
    {

        transform: scaleY(1);
        transform-origin:bottom; 
        transition: transform 0.5s;
    
    }

    .cont .box h2
    {
        position: absolute;
        left: 40px;
        top: 70px;
        font-size: 4em;
        font-weight:800;
        z-index: 1;
        opacity: 0.1;
        transition: 0.5s;

    }
    .cont .box img
    {
        position: absolute;
        left: 25px;
        top: 0px;
        font-size: 4em;
        width:230px;
        height:130px;  
        z-index: 1;
        opacity: 1;
        transition: 0.5s;
        margin-top:11%;

    }
    .cont .box:hover img
    {
        width:100px;
        height:90px; 
        border-radius:950px; 
        position: absolute;
        left:150px;
        top:10px;

    }

    .cont .box:hover h2
    {
        opacity: 1;
        color: #fff;
        transform: translateY(-50px);

    }
    .cont .box h3
    {
        position: relative;
        font-size:1.5em;
        z-index: 2;
        color: #fff;
        transition: 0.5s; 
        padding-top:40%; 

      
    }

    .cont .box p
    {
        position: relative;
        z-index: 2;
        color: #fff;
        transition: 0.5s;
        font-size:18px;

    }
    .cont .box button
    {
            position: relative;
            z-index: 2;
            transition: 0.5s;
            background: #cc0a0a;
            color: #fff;
            border: none;
            box-shadow: none;
            padding: 10px;
            width: 100%;
            cursor:pointer;
    }


   .cont .box:hover h3,
   .cont .box:hover p,
   .cont .box:hover button
    {
        transform: translateY(-50px);
        color:#fff; 
    }

    .cont .box:hover button{
        background-color: #fff;
        color: #161819;
        font-weight:700
    }


</style>
