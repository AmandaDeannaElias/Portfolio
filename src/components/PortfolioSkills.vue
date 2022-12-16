<template>
  <div id="skills" >
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
      <div class="two_card_rows">
        <div class="flip-card">
          <div class="flip-card-inner">
            <div class="flip-card-front">
              <div class="skill_name">Vue.js</div>
            </div>
            <div class="flip-card-back">
              <p>
                 I love Vue.js. It's simple and reusable with its component based architecture allowing 
                 everything to be developed in a single page. Bonus: I love how I can conditionally render 
                 elements inline, it saves a lot of time.
              </p>
            </div>
          </div>
        </div>
        <div class="flip-card">
          <div class="flip-card-inner">
            <div class="flip-card-front">
              <div class="skill_name_long">WordPress</div>
            </div>
            <div class="flip-card-back">
              <p>
                WordPress has become part of my daily code stack for the past year and a half. It's
                user friendly and a great tool for businesses to be able to showcase 
                and sell goods, services and more. Much of my WordPress experience includes WPBakery, Yellowpencil, 
                Elementor, Contact Form 7, custom CSS and more.
              </p>
            </div>
          </div>
        </div>
      </div>
      <div class="card_rows">
        <div class="flip-card">
          <div class="flip-card-inner">
            <div class="flip-card-front">
              <div class="skill_name_extra_long">PHP/Laravel</div>
            </div>
            <div class="flip-card-back">
              <p>
                My back-end experience is heavily based in PHP and Laravel. I thoroughly enjoy using Laravel as it
                 makes coding easier through its MVC architecture, migrations and easy API integration. As someone who creates APIs everyday,
                  it's a feature I've grown to love.
              </p>
            </div>
          </div>
        </div>
        <div class="flip-card">
          <div class="flip-card-inner">
            <div class="flip-card-front">
              <div class="skill_name_full_length">API Development</div>
            </div>
            <div class="flip-card-back">
              <p>
                APIs are incredibly useful. Whether its used internally or externally, it makes sending and recieving information
                optimal. I currently use Laravel, Vue.js, Vanilla JS and WordPress to build, GET and POST my REST APIs.
              </p>
            </div>
          </div>
        </div>
        <div class="flip-card">
          <div class="flip-card-inner">
              <div class="flip-card-front">
                <div class="skill_name">MySQL</div>
              </div>
              <div class="flip-card-back">
                <p>
                  Simple and straightforward. DBeaver is my weapon of choice at the moment.
                </p>
              </div>
          </div>
        </div>
      </div>
      <div>
        <h3 class="other_skills_list">Other skills include: Git, jQuery and AWS</h3>
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
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Marcellus&family=Work+Sans:wght@300&display=swap');

.skills_wrapper{
  padding-right: 2vw;
  padding-left: 2vw;
  padding-bottom: 5vh;
  animation: fadeIn ease 4s;
  -webkit-animation: fadeIn ease 4s;
  -moz-animation: fadeIn ease 4s;
  -o-animation: fadeIn ease 4s;
  -ms-animation: fadeIn ease 4s;
}

h3{
  font-family: 'Marcellus', serif;
  font-size:2.5em;
  font-weight: normal;
  color:#dbd7d0;
  text-align:center;
  line-height: 1em;
  padding-right: 2vw;
  padding-bottom: 5vh;
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
  margin-bottom: 10vh;
}

.two_card_rows{
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
  margin-bottom: 10vh;
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
  font-size: 3.8em;
  padding-right: 20px;
}

.skill_name_long{
  font-size: 3.2em;
  padding-right: 3px;
}

.skill_name_extra_long{
  font-size: 2.8em;
  padding-right: 3px;
}

.skill_name_full_length{
  font-size: 2.4em;
}

.other_skills_list{
  font-family: 'Marcellus', serif;
  font-size: 1.5em;
  font-weight: normal;
  color:#dbd7d0;
  text-align:center;
  line-height: 1em;
  padding-right: 2vw;
  padding-top: 2vw;
  padding-bottom: 5vh;
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

.fadeIn{ 
  opacity: 1; 
}

.fade{
  transition: 0.8s ease-in;
}

@media screen and (min-width: 1750px){
  .card_rows{
    justify-content: space-evenly;
  }
  h3{
    font-size:4em;
  }
}
</style>
