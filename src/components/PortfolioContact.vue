<template>
    <div id="contact" class="contact_wrapper">
      <img class="bg_image" src="/images/contactme.jpg" />
      <div class="two_columns">
        <div class="first_column">
          <h2 class="h2_class">Contact Me</h2>
          <h3 class="h3_class">Feel free to check out my GitHub, send me a connection on LinkedIn  or 
            even just say hello. I'd love to hear from you.
          </h3>
        </div>
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
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Marcellus&family=Work+Sans:wght@300&display=swap');

.contact_wrapper{
  padding-right: 2vw;
  padding-left: 2vw;
  padding-bottom: 15vh;
  padding-top: 10vh;
  position: relative;
}

.bg_image{
  opacity: 0.2;
  position: absolute;
  pointer-events: none;
  left: 0;
  top: 0;
  width: 100%;
  -webkit-filter: grayscale(100%);
  filter: grayscale(95%);
  max-height: 600px;
}

.two_columns{
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
  align-items: center;
  position: relative;
}

.h3_class{
  font-family: 'Marcellus', serif;
  font-size:2em;
  font-weight: normal;
  color:#dbd7d0;
  text-align:left;
  line-height: 1em;
  padding-right: 2vw;
  padding-top: 2vw;
  padding-bottom: 5vh;
}

.first_column{
  width: 55%;
  padding-left: 2vh;
  padding-bottom: 2vh;
  border-left: 2px #dbd7d0 solid; 
  border-bottom: 2px #dbd7d0 solid;
}

.h2_class{
  font-family: 'Marcellus', serif;
  font-size:2.5em;
  font-weight: normal;
  color:#dbd7d0;
  text-align:center;
  line-height: 1em;
  padding-right: 2vw;
}

.flex_contact{
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  padding-top: 2vw;
  border-right: 2px #dbd7d0 solid; 
  border-top: 2px #dbd7d0 solid;
  padding-right: 2vh;
  padding-top: 2vh;
}

.contact_spacing{
  padding-bottom: 5vh;
}

img{
  margin-right: 1vw;
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

@media screen and (min-width: 1750px){
  .h2_class{
    font-size:4em;
  }

  .h3_class{
    font-size:2.5em;
  }
}

</style>
