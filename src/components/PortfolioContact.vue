<template>
    <div id="contact" class="contact_wrapper fade fadeOut">
      <h2 class="h2_class">Contact Me</h2>
      <div class="two_columns">
        <h3 class="h3_class">Feel free to check out my GitHub, send me a connection on LinkedIn  or 
          even just say hello. I'd love to hear from you.
        </h3>
        <div class="flex_contact">
          <div class="contact_spacing">
            <img src="/images/github.png" height=32/>
            <a href="https://github.com/AmandaDeannaElias" target="_blank">https://github.com/AmandaDeannaElias</a>
          </div>
          <div class="contact_spacing">
            <img src="/images/linkedin.png" height=32/>
            <a href="https://www.linkedin.com/in/amandaelias1" target="_blank">https://www.linkedin.com/in/amandaelias1</a>
          </div>
          <div class="contact_spacing">
            <img src="/images/email.png" height=32/>
            <a href="mailto:amanda.elias@live.ca" target="_blank">amanda.elias@live.ca</a>
          </div>
        </div>
      </div>
    </div>
</template>

<script>
export default {
  name: 'PortfolioContact',
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

.contact_wrapper{
  padding-right: 2vw;
  padding-left: 2vw;
  padding-bottom: 25vh;
}

.two_columns{
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
  align-items: center;
}

.h3_class{
  font-family: 'Marcellus', serif;
  font-size:2.5em;
  font-weight: normal;
  color:#dbd7d0;
  text-align:left;
  line-height: 1em;
  padding-right: 2vw;
  padding-top: 2vw;
  padding-bottom: 5vh;
  width: 35%;
}

.h2_class{
  font-family: 'Marcellus', serif;
  font-size:2.5em;
  font-weight: normal;
  color:#dbd7d0;
  text-align:center;
  line-height: 1em;
  padding-right: 2vw;
  padding-top: 2vw;
  padding-bottom: 5vh;
}

.flex_contact{
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  padding-top: 2vw;
}

.contact_spacing{
  padding-bottom: 5vh;
}

img{
  margin-right: 2vw;
}

a {
  position: relative;
  text-decoration: none;
  color: #dbd7d0;
  font-family: 'Marcellus', serif;
  padding: 0 10px;
  letter-spacing: 0.5px;
}

a:after{
  content: '';
  position: absolute;
  height: 1px;
  width: 0;
  left: 0;
  bottom: -10px;
  background-color: #dbd7d0;
  transition: 0.3s;
}

a:hover:after{
  width: 100%;
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
