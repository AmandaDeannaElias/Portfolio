<template>
    <nav class="nav_background">
      <img class="bg_image" src="/images/js2.jpg" />
      <div class="nav_menu">
        <div></div>
        <h1 class="headings my_name zoom">Amanda Elias</h1>
        <ul>
          <li class="zoom"><a href="#about" rel="noopener">About</a></li>
          <li class="zoom"><a href="#skills" rel="noopener">Skills</a></li>
          <li class="zoom"><a href="#contact" rel="noopener">Contact</a></li>
          <li class="zoom"><a href="https://github.com/AmandaDeannaElias" target="_blank">Projects (Coming Soon)</a></li>
        </ul>
        <div class="speakers">
          <img id="speaker_off" v-if="musicPlaying" @click="musicOn()" height="20" src="/images/speaker_off.png"/>
          <img id="speaker_on" v-if="musicOff" @click="musicPause()" height="20" src="/images/speaker_on.png"/>
        </div>
      </div>
    </nav>
</template>

<script>
export default {
  name: 'PortfolioHeader',
  props: {
    msg: String
  },

  data() {
    return{
      musicPlaying: true,
      musicOff: false,
      audio: new Audio("/music/lofi-3.mp3"),
    }
  },

  methods: {

      musicOn(){
        this.musicPlaying = false;
        this.audio.play();
        this.musicOff = true;
        this.audio.loop = true;
      },

      musicPause(){
        this.musicOff = false;
        this.musicPlaying = true;
        this.audio.pause();
      }
  }
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Marcellus&family=Work+Sans:wght@300&display=swap');

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
  font-size: 1.7em;
}

a {
  position: relative;
  text-decoration: none;
  color: #dbd7d0;
  font-family: 'Marcellus', serif;
  padding: 0 10px;
  letter-spacing: 0.5px;
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
}

.nav_background{
  position: relative;
}

.speakers{
  cursor: pointer;
}

#speaker_on{
  animation: zoom-in-zoom-out 2s ease infinite;
}

@keyframes zoom-in-zoom-out {
  0% {
    transform: scale(1, 1);
  }
  50% {
    transform: scale(1.5, 1.5);
  }
  100% {
    transform: scale(1, 1);
  }
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

.nav_menu{
  display:flex;
  justify-content: space-between;
  align-items: flex-end;
  padding-top:10vh;
  padding-left:2vw;
  padding-right:2vw;
  padding-bottom:5vh;
  
}

.my_name{
  font-family: 'Marcellus', serif;
  margin-top: 0;
  margin-bottom:0;
  font-size:3em;
  font-weight: normal;
  position: relative;
  text-decoration: none;
  color: #dbd7d0;
  font-family: 'Marcellus', serif;
  padding: 0 10px;
  letter-spacing: 0.5px;
  cursor: default;
}

.my_name:after{
  content: '';
  position: absolute;
  height: 1px;
  width: 0;
  left: 0;
  bottom: -10px;
  background-color: #dbd7d0;
  transition: 0.3s;
}

.my_name:hover:after{
  width: 100%;
}

.zoom {
  transition: transform .3s;
}

.zoom:hover{
  transform: scale(1.1);
}

@media screen and (max-width: 1400px){
  .bg_image{
    height:180vh;
  }
}
@media screen and (min-width: 1750px){
  li{
    font-size: 2.2em;
  }
  .my_name{
    font-size: 3.5em;
  }
}
</style>
