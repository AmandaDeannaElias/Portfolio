<template>
    <div class="opening_wrapper fade fadeOut">
      <div class="wrap_masonry">
        <div class="image_div image_animation">
          <img src="/images/toronto5.jpg" width=375 alt="Toronto Landscape" id="toronto_landscape_image" title="Toronto Landscape"/>
          <img src="/images/meatdesk.jpg" width=125 alt="Me smiling at my desk" id="me_at_desk_image" title="Toronto Landscape"/>
        </div>
        <div class="image_div_second image_animation">
          <img src="/images/flowers.jpg" width=150 alt="White daffodils" id="flowers_image" title="Toronto Landscape"/>
          <img src="/images/laptop.jpg" width=350 alt="A coffee with a macbook" id="laptop_image" title="Toronto Landscape"/>
        </div>
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
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Marcellus&family=Work+Sans:wght@300&display=swap');

.opening_wrapper{
  display: flex;
  padding-right: 5vw;
  padding-left: 5vw;
  padding-bottom: 15vh;
  position: relative;
}

.wrap_masonry{
  padding-left: 2vh;
  padding-bottom: 2vh;
  border-left: 2px #dbd7d0 solid; 
  border-bottom: 2px #dbd7d0 solid;
  width:60%;
}

.image_div{
  width: 100%;
  opacity: 100%;
  display: flex;
  flex-direction: row;
  padding-left: 2vh;
  padding-bottom: 2vh;
}

.image_div_second{
  width: 100%;
  opacity: 100%;
  display: flex;
  flex-direction: row;
  padding-left: 2vh;
  padding-bottom: 2vh;
}

.image_div img{
  opacity: 100%;
}

#me_at_desk_image{
  margin-left: 2vw;
}

#laptop_image{
  margin-left: 2vw;
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
  width:40%;
}

img{
  float: left;
  filter:grayscale(60%);
  max-width: 100%;
  display: block;
  border-radius: 8px;
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

@media screen and (min-width: 1750px){
  h3{
    font-size:3.5em;
  }
  #toronto_landscape_image{
    width: 550px;
  }
  #me_at_desk_image{
    width: 175px;
  }
  #flowers_image{
    width: 250px;
  }
  #laptop_image{
    width: 475px;
  }
  .opening_wrapper{
    padding-right: 10vw;
    padding-left: 10vw;
  }
}
</style>
