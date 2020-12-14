<template>
  <div class="container top-117" id="Portfolio">
      <div class="col-md-12">

          <div class="row display_flex_justify_center p-t-80">
    
           <div class="text-center">
               <h1 v-if="this.$parent.leneng">Portfolio</h1>
               <h1 v-if="this.$parent.lenfrench">Prés Traveaux</h1>
           </div>

         </div>

         <div class="row p-t-50">
               <div class="col-md-6 pos-relative project-container">
                 <img src="images/artdevportfolio/sahabmockup.png"  class="col " alt="">
                 <div class="img-overlay">
                     <button @click="redirctto(0)" v-if="this.$parent.leneng">View Project</button>
                     <button @click="redirctto(0)" v-if="this.$parent.lenfrench">Voir le Projet</button>
                 </div>
             </div>

               <div class="col-md-6 pos-relative project-container">
                 <img src="images/artdevportfolio/sahabblogmockup.png"  class="col " alt="">
                 <div class="img-overlay">
                     <button @click="redirctto(1)" v-if="this.$parent.leneng">View Project</button>
                     <button @click="redirctto(1)" v-if="this.$parent.lenfrench">Voir le Projet</button>
                 </div>
             </div>

         </div>

         <div class="row display_flex_justify_center p-t-50">
               <div class="col-md-6 pos-relative project-container">
                 <img src="images/artdevportfolio/ishopmockup.png"  class="col " alt="">
                 <div class="img-overlay">
                     <button @click="redirctto(2)" v-if="this.$parent.leneng">View Project</button>
                     <button @click="redirctto(2)" v-if="this.$parent.lenfrench">Voir le Projet</button>
                 </div>
             </div>

         </div>

          <div class="row p-t-50">
               <div class="col-md-6 pos-relative project-container">
                 <img src="images/artdevportfolio/elmaalim.png"  class="col " alt="">
                 <div class="img-overlay">
                     <button @click="redirctto(3)" v-if="this.$parent.leneng">View Project</button>
                     <button @click="redirctto(3)" v-if="this.$parent.lenfrench">Voir le Projet</button>
                 </div>
             </div>

               <div class="col-md-6 pos-relative project-container">
                 <img src="images/artdevportfolio/studyeverywhere.png"  class="col " alt="">
                 <div class="img-overlay">
                    <button @click="redirctto(4)" v-if="this.$parent.leneng">View Project</button>
                     <button @click="redirctto(4)" v-if="this.$parent.lenfrench">Voir le Projet</button>
                 </div>
             </div>

         </div>

      </div>
  </div>
</template>

<script>
export default {
  name: 'Portfolio',
  data(){
      return{
          links:[
              "https://sahaaab.com",
              "https://blog.sahaaab.com",
              "http://abdoudesign.epizy.com",
              "https://almaealim.com/",
              "https://abdoutony.github.io/bootstrap_landing_page_educational_website/"
          ]
      }
  },
  methods:{
    redirctto(id){
            window.open(this.links[id], '_blank');
    }
  }
 
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.img-overlay{
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: #1618198c;
    display: flex;
    justify-content: center;
    align-items: center;
    display: none;
}

.img-overlay button{
     position: relative;
            z-index: 2;
            transition: 0.5s;
            background: #cc0a0a;
            color: #fff;
            border: none;
            box-shadow: none;
            padding: 10px;
            padding-left: 30px;
            padding-right: 30px;
            cursor:pointer;
}

.project-container:hover .img-overlay{
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: #1618198c;
    display: flex;
    justify-content: center;
    align-items: center;
}
</style>
