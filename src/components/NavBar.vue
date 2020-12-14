<template>
  <div class="container-fluid navbar-container upper_nav" id="Home">
     <div class="col-md-12">
         <div class="row">              
              <nav class="navbar navbar-expand-lg col-md-12  ">
                <a href="#" class="navbar-brand">
                    <img src="/images/artdevlogofinalwhite.png" alt="logo" width="150">
                </a>
                <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
                <i class="fas fa-list"></i>
              </button>
             <div class="collapse navbar-collapse " id="navbarSupportedContent">
                 <ul class="navbar-nav ml-auto links m-b-0">
                    <li class="nav-item" >
                    <a @click="navigateTo(0)"  class="link" ref="l0">
                        <span v-if="this.$parent.leneng">Home</span>
                        <span v-if="this.$parent.lenfrench">Acceuil</span>
                        <div class="line yellow"></div>
                    </a>
                    </li>
                    <li class="nav-item" >
                    <a @click="navigateTo(1)"   class="link" ref="l1">
                       <span v-if="this.$parent.leneng">How It Works</span>
                        <span v-if="this.$parent.lenfrench">Comment Ca Marche</span>
                        <div class="line yellow"></div>
                    </a>
                    </li>
                    <li class="nav-item" >
                    <a @click="navigateTo(2)"  class="link" ref="l2">
                        <span v-if="this.$parent.leneng">Our Services</span>
                        <span v-if="this.$parent.lenfrench">Nos Services</span>
                        <div class="line yellow"></div>
                    </a>
                    </li>
                    <li class="nav-item" >
                    <a @click="navigateTo(3)"  class="link" ref="l3">
                        <span v-if="this.$parent.leneng">Portfolio</span>
                        <span v-if="this.$parent.lenfrench">Prés Traveaux</span>
                        <div class="line yellow"></div>
                    </a>
                    </li>
                    <li class="nav-item" >
                    <a @click="navigateTo(4)"  class="link" ref="l4">
                        <span>Contacts</span>
                        <div class="line yellow"></div>
                    </a>
                    <li class="nav-item" >
                     <a @click="changeLanguageToFrench" v-if="this.$parent.leneng" class="link" ref="l4">
                        <span>Francais</span>
                        <div class="line yellow"></div>
                    </a>
                     <a @click="changeLanguageToEnglish" v-if="this.$parent.lenfrench"  class="link" ref="l4">
                        <span>English</span>
                        <div class="line yellow"></div>
                    </a>
                    </li>
                </ul>
             </div>
              </nav>
         </div>
     </div>
  </div>
</template>

<script>
import $ from 'jquery'
export default {

  name: 'NavBar',
 
   data(){
      return {
          ids: ["app", "HowItWorks", "OurServices", "Portfolio", "Contacts"],
         
      }
  },
  methods:{
    changeLanguageToFrench(){
       this.$parent.lenfrench = true
       this.$parent.leneng = false
    },
     changeLanguageToEnglish(){
       this.$parent.leneng = true
       this.$parent.lenfrench = false
    },
     navigateTo: function (id) {
    //  const linkRef = this.$refs.l0;
    //  linkRef.focus();
     // this.$set(this.$data, "section", id);
      document.querySelector("#" + this.$data.ids[id]).scrollIntoView({
        behavior: "smooth",
      });
    },
    ChangNavbarOnScroll(){
        
       $(function() {
    var header = $(".upper_nav");
    $(window).scroll(function() {    
        var ss = $(window).scrollTop();
    
        if (ss >= 100) {
            header.removeClass('upper_nav').addClass("upper_nav1");
        } else {
            header.removeClass("upper_nav1").addClass('upper_nav');
        }
    });
});
    }
  },
  mounted(){
    $(document).ready(function(){
    $(this).scrollTop(0);
     }); 
   this.ChangNavbarOnScroll()
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
   
   .navbar-toggler{
     background: #ffffff;
     color: #161819;
   }
   .navbar-toggler-icon{
     background: #161819;
   }
  
   .navbar-container{
       padding:20px;
       position:fixed;
       z-index: 99999;
    
   }

  .upper_nav{
  transition-duration: .5s;
  background-color: #161819;
  padding-bottom: 0 !important;
}

.upper_nav1{
  background:#161819;
  color:#fff;
  padding:0px;
  padding-right: 10px;
  box-shadow: 0px 1px 4px #fff;
}

   .line {
  width: 0%;
  height: 5px;
  transition: ease-out 0.5s;
  margin-left: auto;
}

.line.yellow {
  background-color: #CC0A0A;
}
.links{
  margin-bottom: 0;
}

.links li.active {
  opacity: 1 !important;
}

li.active .line {
  width: 100% !important;
  margin-right: auto;
  margin-left: 0px;
}

.links {
  list-style: none;
}

.link {
  color: white;

  font-size: 18px;
  cursor: pointer;
}

.links li {
  float: left;
  padding-left: 40px;
  transition: ease-out 0.25s;
}


.links li:hover .line {
  width: 100%;
  margin-right: auto;
  margin-left: 0px;
}

.links li:hover {
  opacity: 1;
}
</style>
