<template>
    <div class="skills_wrapper fade fadeOut">
      <div class="h3_skills_section">
        <h3>Skills</h3>
      </div>
      <div class="card_rows">
        <div class="flip-card">
          <div class="flip-card-inner">
            <div class="flip-card-front">
              <div class="skill_name">JS</div>
            </div>
            <div class="flip-card-back">
              <p>
                One of the first languages I learned was Vanilla JavaScript during my time at Humber College.
                I started using this language to simply manipulate the DOM, and currently use it to consume APIs, 
                create custom validation and add emphasis to design.
              </p>
            </div>
          </div>
        </div>
        <div class="flip-card">
          <div class="flip-card-inner">
              <div class="flip-card-front">
                <div class="skill_name">HTML</div>
              </div>
              <div class="flip-card-back">
                <p>
                  HTML was the very first language I worked with as many developers do. It gets a bad reputation 
                  for being a boring language, but we wouldn't have webpages without it. It's constantly evolving 
                  to become more accessible; that's something I appreciate.
                </p>
              </div>
          </div>
        </div>
        <div class="flip-card">
          <div class="flip-card-inner">
            <div class="flip-card-front">
              <div class="skill_name">CSS</div>
            </div>
            <div class="flip-card-back">
              <p>
                CSS has become one of my favourite languages to work with. There are endless possibilities for design 
                including animations and responsiveness. CSS is one of the most powerful tools to engage users and invoke
                creativity. HTML is the canvas, and CSS is the paint.
              </p>
            </div>
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
  padding-bottom: 10vh;
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
  height: 225px;
  perspective: 1000px;
  cursor: pointer;
}

.card_rows{
  display: flex;
  flex-direction: row;
  justify-content: space-around;
}

.flip-card-inner {
  position: relative;
  width: 100%;
  height: 100%;
  text-align: center;
  transition: transform 0.8s;
  transform-style: preserve-3d;
}

.flip-card:hover .flip-card-inner {
  transform: rotateY(180deg);
}

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
}

.flip-card-back {
  background-color: #dbd7d0;
  display: flex;
  align-items: center;
  padding: 10px 10px 10px 10px;
  transform: rotateY(180deg);
  font-size: 1em;
  font-family: 'Work Sans', sans-serif;
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
