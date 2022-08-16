<template>
  <header>
    <div class="nav_menu">
      <div></div>
      <h1 class="headings my_name zoom"><a href="#" target="_blank" rel="noopener">Amanda Elias</a></h1>
      <ul>
        <li class="zoom"><a href="#" target="_blank" rel="noopener">About</a></li>
        <li class="zoom"><a href="#" target="_blank" rel="noopener">Skills</a></li>
        <li class="zoom"><a href="#" target="_blank" rel="noopener">Contact</a></li>
      </ul>
    </div>
  </header>
</template>

<script>
export default {
  name: 'PortfolioHeader',
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
ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
  font-size: 2em;
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

.nav_menu{
  display:flex;
  justify-content: space-between;
  align-items: flex-end;
  padding-top:10vh;
  padding-left:2vw;
  padding-right:2vw;
}

.my_name{
  color: #dbd7d0;
  font-family: 'Marcellus', serif;
  margin-top: 0;
  margin-bottom:0;
  font-size:3em;
  font-weight: normal;
}

.zoom {
  transition: transform .3s;
}

.zoom:hover{
  transform: scale(1.1);
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

</style>
