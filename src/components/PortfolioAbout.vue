<template>
    <div class="about_wrapper fade fadeOut">
      <div class="about_list_container">
        <div class="about_border">
          <h3>About</h3>
          <div class="about_list">
            <p class="plus_sign">&#43;&nbsp; </p>
            <p> A woman in tech who loves her job</p>
          </div>
          <div class="about_list">
            <p class="plus_sign">&#43;&nbsp; </p>
            <p> Graduated from Humber College for the Web Development program</p>
          </div>
          <div class="about_list">
            <p class="plus_sign">&#43;&nbsp; </p>
            <p> Always learning, staying current and expanding upon my current code stack</p>
          </div>
          <div class="about_list">
            <p class="plus_sign">&#43;&nbsp; </p>
            <p> Free time includes music, cooking, gaming and exploring other cultures</p>
          </div>
        </div>
        <img src="/images/Me.jpg" height=400/>
      </div>
    </div>
</template>

<script>
export default {
  name: 'PortfolioBio',
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
@import url('https://fonts.googleapis.com/css2?family=Marcellus&family=Work+Sans:wght@400&display=swap');

.about_wrapper{
  background-color: #1a1a1a;
  padding-bottom: 30vh;
  padding-right: 2vw;
  padding-left: 2vw;
}

.about_title{
  display: flex;
  justify-content: space-around;
  padding-bottom: 5vh;
}

.about_border{
  padding-left: 2vh;
  padding-bottom: 2vh;
  border-left: 2px #dbd7d0 solid; 
  border-bottom: 2px #dbd7d0 solid;
}

.about_list_container{
  display: flex;
  justify-content: space-around;
}

.about_list{
  display: flex;
  align-items: center;
  flex-direction: row;
}

.animation{
  animation: fadeIn ease 4s;
  -webkit-animation: fadeIn ease 4s;
  -moz-animation: fadeIn ease 4s;
  -o-animation: fadeIn ease 4s;
  -ms-animation: fadeIn ease 4s;
  background-color: #dbd7d0;
  padding-top: 12vh;
  padding-bottom: 12vh;
}

h3{
  font-family: 'Marcellus', serif;
  font-size: 3.5em;
  font-weight: normal;
  color:#dbd7d0;
  line-height: 1em;
  padding-right: 2vw;
  padding-bottom: 5vh;
}

img{
  border-right: 2px #dbd7d0 solid; 
  border-top: 2px #dbd7d0 solid;
  padding-right: 2vh;
  padding-top: 2vh;
}

.plus_sign{
  font-weight: bolder;
  font-size: 2.5em;
}

p{
  font-family: 'Work Sans', sans-serif;
  font-size: 1.2em;
  font-weight: normal;
  color:#dbd7d0;
  line-height: 1.5em;
  text-align:left;
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
