<template>
    <div class="opening_wrapper fade fadeOut">
      <div class="image_div image_animation">
        <img src="/images/Toronto.jpg" alt="Toronto Landscape" title="Toronto Landscape"/>
      </div>
      <div class="h3_column">
        <h3 class="first_h3_animation"> Nice to see you here. </h3>
        <h3 class="second_h3_animation"> My name is Amanda Elias. </h3>
        <h3 class="third_h3_animation"> I am a Toronto-based Web Developer. </h3>
      </div>
    </div>
</template>

<script>
export default {
  name: 'PortfolioOpening',
  props: {
    msg: String
  },

  mounted: function(){
    
  },

  methods: {

  }
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Marcellus&family=Work+Sans:wght@300&display=swap');

.opening_wrapper{
  display: flex;
  padding-right: 2vw;
  padding-left: 2vw;
  padding-bottom: 15vh;
  position: relative;
}

.image_div{
  width: 100%;
  opacity: 100%;
}

.image_div img{
  opacity: 100%;
}

.image_animation{
  animation: fadeIn ease 3s;
  -webkit-animation: fadeIn ease 3s;
  -moz-animation: fadeIn ease 3s;
  -o-animation: fadeIn ease 3s;
  -ms-animation: fadeIn ease 3s;
}

h3{
  font-family: 'Marcellus', serif;
  font-size:2.5em;
  font-weight: normal;
  color:#dbd7d0;
  text-align:right;
  line-height: 1em;
  padding-right: 2vw;
  padding-top:2vh;
}

.h3_column{
  flex-direction: column;
  border-right: 2px #dbd7d0 solid; 
  border-top: 2px #dbd7d0 solid;
  opacity: 100%;
}

img{
  float: left;
  width: 90%;
  opacity: 0.8;
  padding-left: 2vh;
  padding-bottom: 2vh;
  border-left: 2px #dbd7d0 solid; 
  border-bottom: 2px #dbd7d0 solid;
}

@keyframes fadeIn {
  0% {
    opacity:0;
  }
  100% {
    opacity:1;
  }
}

@-moz-keyframes fadeIn {
  0% {
    opacity:0;
  }
  100% {
    opacity:1;
  }
}

@-webkit-keyframes fadeIn {
  0% {
    opacity:0;
  }
  100% {
    opacity:1;
  }
}

@-o-keyframes fadeIn {
  0% {
    opacity:0;
  }
  100% {
    opacity:1;
  }
}

@-ms-keyframes fadeIn {
  0% {
    opacity:0;
  }
  100% {
    opacity:1;
}
}

.fadeOut{ 
  opacity: 0; 
}

.fadeIn{ 
  opacity: 1; 
}

.fade{
  transition: 0.8s ease-in;
}

</style>
