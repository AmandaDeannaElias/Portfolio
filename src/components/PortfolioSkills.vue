<template>
    <div class="skills_wrapper fade fadeOut">
      <div class="h3_skills_section">
        <h3>Skills</h3>
      </div>
      <div class="flip-card">
        <div class="flip-card-inner">
          <div class="flip-card-front">
            <div class="skill_name">JS</div>
          </div>
          <div class="flip-card-back">
            <h1>John Doe</h1>
            <p>Architect & Engineer</p>
            <p>We love that guy</p>
          </div>
        </div>
      </div>
    </div>
</template>

<script>
export default {
  name: 'PortfolioSkills',
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

.skills_wrapper{
  padding-right: 2vw;
  padding-left: 2vw;
  padding-bottom: 15vh;
}

h3{
  font-family: 'Marcellus', serif;
  font-size:2.5em;
  font-weight: normal;
  color:#dbd7d0;
  text-align:center;
  line-height: 1em;
  padding-right: 2vw;
  padding-top: 2vw;
}

.h3_column{
  flex-direction: column;
  border-right: 2px #dbd7d0 solid; 
  border-top: 2px #dbd7d0 solid;
  animation: fadeIn ease 9s;
  -webkit-animation: fadeIn ease 9s;
  -moz-animation: fadeIn ease 9s;
  -o-animation: fadeIn ease 9s;
  -ms-animation: fadeIn ease 9s;
}

.flip-card {
  background-color: transparent;
  width: 250px;
  height: 200px;
  perspective: 1000px;
}

/* This container is needed to position the front and back side */
.flip-card-inner {
  position: relative;
  width: 100%;
  height: 100%;
  text-align: center;
  transition: transform 0.8s;
  transform-style: preserve-3d;
}

/* Do an horizontal flip when you move the mouse over the flip box container */
.flip-card:hover .flip-card-inner {
  transform: rotateY(180deg);
}

/* Position the front and back side */
.flip-card-front, .flip-card-back {
  position: absolute;
  width: 100%;
  height: 100%;
  -webkit-backface-visibility: hidden;
  backface-visibility: hidden;
  border-radius: 8px;
  font-family: 'Marcellus', serif;
}

.flip-card-front {
  background-color: #dbd7d0;
  display: flex;
  align-items: flex-end;
  justify-content: flex-end;
  padding-right: 30px;
  padding-bottom: 20px;
}

/* Style the back side */
.flip-card-back {
  background-color: #dbd7d0;
  display: flex;
  align-items: flex-end;
  justify-content: flex-end;
  padding-right: 30px;
  padding-bottom: 20px;
  transform: rotateY(180deg);
}

.skill_name{
  font-size: 4.5em;
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
