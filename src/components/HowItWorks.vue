<template>
  <div class="container-fluid top-117" id="HowItWorks">
     <div class="col-md-12">
         <div class="row display_flex_justify_center p-t-80">
    
           <div class="text-center">
               <h1 v-if="this.$parent.leneng">How It Works</h1>
               <h1 v-if="this.$parent.lenfrench">Comment Ca Marche</h1>
           </div>

         </div>

         <div class="row">


             <!-- The Timeline -->

<ul class="timeline">

	<!-- Item 1 -->
	<li>
		<div class="direction-r">
			<div class="flag-wrapper">
				<h5 v-if="this.$parent.leneng" class="flag">Find the service</h5>
			<h5 v-if="this.$parent.lenfrench" class="flag">Chercher le service</h5>
			</div>
			<div v-if="this.$parent.leneng" class="desc">
        Look for the service you want, we provide a lot of service in several areas
       </div>
       <div v-if="this.$parent.lenfrench" class="desc">
      Chercher bien le service que vous souhaité on realise pas mal de service dans plusieur domaines
       </div>
		</div>
	</li>
  
	<!-- Item 2 -->
	<li>
		<div class="direction-l">
			<div class="flag-wrapper">
				<h5 v-if="this.$parent.leneng" class="flag">Make a coffee with us</h5>
				<h5 v-if="this.$parent.lenfrench" class="flag">Fait un café avec nous</h5>
			
			</div>
			<div v-if="this.$parent.leneng" class="desc">
      Book your appointment to speak with our manager to explain your project well
      </div>
      <div v-if="this.$parent.lenfrench" class="desc">
     Réservez votre rendez vous pour parler avec notre mangere pour lui explique bien votre projet
      </div>
		</div>
	</li>

	<!-- Item 3 -->
	<li>
		<div class="direction-r">
			<div class="flag-wrapper">
				<h5 v-if="this.$parent.leneng" class="flag">Receive your project</h5>
				<h5 v-if="this.$parent.lenfrench" class="flag">Recevez votre projet</h5>
				
			</div>
			<div v-if="this.$parent.leneng" class="desc">
      We have a team that works day and night to complete your project within the time limit
      </div>
      <div v-if="this.$parent.lenfrench" class="desc">
      Nous avons une équipe qui travail jours et nuit a fin de completer votre projet dans le delai
      </div>
		</div>
	</li>
  
</ul>


         </div>
     </div>
  </div>
</template>

<script>
export default {
  name: 'HowItWorks'
 
 
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>



/* ================ The Timeline ================ */

.timeline {
  position: relative;
  width: 660px;
  margin: 0 auto;
  margin-top: 20px;
  padding: 1em 0;
  list-style-type: none;
}

.timeline:before {
  position: absolute;
  left: 50%;
  top: 0;
  content: ' ';
  display: block;
  width: 6px;
  height: 100%;
  margin-left: -3px;
  background: #fff;
/* background: -moz-linear-gradient(top, rgba(80,80,80,0) 0%, rgb(80,80,80) 8%, rgb(80,80,80) 92%, rgba(80,80,80,0) 100%);
  background: -webkit-gradient(linear, left top, left bottom, color-stop(0%,rgba(30,87,153,1)), color-stop(100%,rgba(125,185,232,1)));
  
  background: -webkit-linear-gradient(top, rgba(80,80,80,0) 0%, rgb(80,80,80) 8%, rgb(80,80,80) 92%, rgba(80,80,80,0) 100%);
  background: -o-linear-gradient(top, rgba(80,80,80,0) 0%, rgb(80,80,80) 8%, rgb(80,80,80) 92%, rgba(80,80,80,0) 100%);
  background: -ms-linear-gradient(top, rgba(80,80,80,0) 0%, rgb(80,80,80) 8%, rgb(80,80,80) 92%, rgba(80,80,80,0) 100%);
  background: linear-gradient(to bottom, rgba(80,80,80,0) 0%, rgb(80,80,80) 8%, rgb(80,80,80) 92%, rgba(80,80,80,0) 100%);
 */ 
  z-index: 5;
}

.timeline li {
  padding: 1em 0;
}

.timeline li:after {
  content: "";
  display: block;
  height: 0;
  clear: both;
  visibility: hidden;
}

.direction-l {
  position: relative;
  width: 300px;
  float: left;
  text-align: right;
}

.direction-r {
  position: relative;
  width: 300px;
  float: right;
}

.flag-wrapper {
  position: relative;
  display: inline-block;
  
  text-align: center;
}

.flag {
  position: relative;
  display: inline;
  background:#cc0a0a;
  padding: 6px 10px;
  border-radius: 5px;
  color:#fff;
  text-align: left;
}

.direction-l .flag {
  -webkit-box-shadow: -1px 1px 1px rgba(0,0,0,0.15), 0 0 1px rgba(0,0,0,0.15);
  -moz-box-shadow: -1px 1px 1px rgba(0,0,0,0.15), 0 0 1px rgba(0,0,0,0.15);
  box-shadow: -1px 1px 1px rgba(0,0,0,0.15), 0 0 1px rgba(0,0,0,0.15);
}

.direction-r .flag {
  -webkit-box-shadow: 1px 1px 1px rgba(0,0,0,0.15), 0 0 1px rgba(0,0,0,0.15);
  -moz-box-shadow: 1px 1px 1px rgba(0,0,0,0.15), 0 0 1px rgba(0,0,0,0.15);
  box-shadow: 1px 1px 1px rgba(0,0,0,0.15), 0 0 1px rgba(0,0,0,0.15);
}

.direction-l .flag:before,
.direction-r .flag:before {
  position: absolute;
  top: 50%;
  right: -37px;
  content: ' ';
  display: block;
  width: 12px;
  height: 12px;
  margin-top: -10px;
  background: #fff;
  border-radius: 10px;
  border: 4px solid #cc0a0a;
  z-index: 10;
}

.direction-r .flag:before {
  left: -35px;
}

.direction-l .flag:after {
  content: "";
  position: absolute;
  left: 100%;
  top: 50%;
  height: 0;
  width: 0;
  margin-top: -8px;
  border: solid transparent;
  border-left-color: #fff;
  border-width: 8px;
  pointer-events: none;
}

.direction-r .flag:after {
  content: "";
  position: absolute;
  right: 100%;
  top: 50%;
  height: 0;
  width: 0;
  margin-top: -8px;
  border: solid transparent;
  border-right-color: #fff;
  border-width: 8px;
  pointer-events: none;
}

.time-wrapper {
  display: inline;
  
  line-height: 1em;
  font-size: 0.66666em;
  color: rgb(250,80,80);
  vertical-align: middle;
}

.direction-l .time-wrapper {
  float: left;
}

.direction-r .time-wrapper {
  float: right;
}

.time {
  display: inline-block;
  padding: 4px 6px;
  background: rgb(248,248,248);
}

.desc {
  margin: 1em 0.75em 0 0;
  
  font-size: 18px;
  line-height: 1.5em;
}

.direction-r .desc {
  margin: 1em 0 0 0.75em;
}





 


@media only screen and (max-width: 660px) {
.timeline {
width: 100% !important;
padding: 4em 0 1em 0 !important;
}

.timeline li {
	padding: 2em 0 !important;
}

.direction-l,
.direction-r {
	float: none !important;
	width: 100% !important;

	text-align: center !important;
}

.flag-wrapper {
	text-align: center !important;
}

.flag {
	background: #cc0a0a !important;
  color:#fff  !important;
	z-index: 15 !important;
}

.direction-l .flag:before,
.direction-r .flag:before {
  position: absolute !important;
  top: -30px !important;
	left: 50% !important;
	content: ' ' !important;
	display: block !important;
	width: 12px !important;
	height: 12px !important;
	margin-left: -6px !important;
	background: #fff !important;
	border-radius: 10px !important;
  border: 4px solid #cc0a0a !important;
	z-index: 10 !important;
}

.direction-l .flag:after,
.direction-r .flag:after {
	content: "" !important;
	position: absolute !important;
	left: 50% !important;
	top: -8px !important;
	height: 0 !important;
	width: 0 !important;
	margin-left: -8px !important;
	border: solid transparent !important;
	border-bottom-color: #FFF !important;
	border-width: 8px !important;
	pointer-events: none !important;
}

.time-wrapper {
	display: block !important ;
	position: relative !important;
	margin: 4px 0 0 0 !important;
	z-index: 14 !important;
}

.direction-l .time-wrapper {
	float: none !important;
}

.direction-r .time-wrapper {
	float: none !important;
}

.desc {
	position: relative !important;
	margin: 1em 0 0 0 !important;
	padding: 1em !important;
  color: #161819;
	background: rgb(245,245,245) !important;
	-webkit-box-shadow: 0 0 1px rgba(0,0,0,0.20) !important;
	-moz-box-shadow: 0 0 1px rgba(0,0,0,0.20) !important;
	box-shadow: 0 0 1px rgba(0,0,0,0.20) !important;
	
  z-index: 15;
}

.direction-l .desc,
.direction-r .desc {
	position: relative;
	margin: 1em 1em 0 1em !important;
	padding: 1em !important;
	
  z-index: 15 !important;
}

}

@media only  screen and (min-width: 400px )and (max-width: 660px) {

.direction-l .desc,
.direction-r .desc {
	margin: 1em 4em 0 4em !important;
}

}






</style>
