<template>
    <div class="bio_wrapper fade fadeOut">
      <!-- <img class="bg_image" src="/images/digital.jpg" /> -->
      <div class="animation">
        <h4 class="h4">Embracing the Digital Age</h4>
        <div class="bio">
          <p></p>
          <p>My journey into web development came at a time where I was craving creative expression.</p>
          <p>Through mentoring from incredible professors, hard work, long hours and dedication, I quickly became addicted to coding.</p>
          <p>Now working in web development, the satisfaction of creating, debugging and collaborating is the real reward.</p>
          <p>There is a solution to every problem. There is a better way to do everything. There is freedom in what you write.</p>
        </div>
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

.bio_wrapper{
  background-color: #1a1a1a;
  display: flex;
  justify-content: center;
  padding-top: 25vh;
  padding-bottom: 25vh;
  padding-right: 9vw;
  padding-left: 9vw;
  position: relative;
  overflow: hidden;
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
  opacity: 100%;
  position: relative;
}


h4{
  font-family: 'Marcellus', serif;
  font-size: 3.5em;
  font-weight: normal;
  color:#1a1a1a;
  line-height: 1em;
  padding-right: 2vw;
  padding-bottom: 3vw;
}

p{
  font-family: 'Work Sans', sans-serif;
  font-size: 1.2em;
  font-weight: normal;
  color:#1a1a1a;
  line-height: 2em;
}
.bio{
  padding-left: 2vw;
  padding-right: 2vw;
}

.bg_image{
  opacity: 0.2;
  position: absolute;
  pointer-events: none;
  left: 0;
  top: 0;
  width: 100%;
  height: 130vh;
  -webkit-filter: grayscale(100%);
  filter: grayscale(100%);
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
