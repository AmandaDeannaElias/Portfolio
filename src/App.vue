<template>
  <PortfolioHeader/>
  <PortfolioOpening/>
  <PortfolioBio/>
  <PortfolioAbout/>
</template>

<script>
import PortfolioHeader from './components/PortfolioHeader.vue'
import PortfolioOpening from './components/PortfolioOpening.vue'
import PortfolioBio from './components/PortfolioBio.vue'
import PortfolioAbout from './components/PortfolioAbout.vue'

export default {
  name: 'App',
  components: {
    PortfolioHeader,
    PortfolioOpening,
    PortfolioBio,
    PortfolioAbout,
  },
  
  mounted: function(){
    const observerOptions = {
      root: null,
      rootMargin: "0px",
      threshold: 0.7
    };

    function observerCallback(entries) {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          entry.target.classList.replace('fadeOut', 'fadeIn');
        } else {
          entry.target.classList.replace('fadeIn', 'fadeOut');
        }
      });
    }
    const observer = new IntersectionObserver(observerCallback, observerOptions);

    const fadeElms = document.querySelectorAll('.fade');
    fadeElms.forEach(el => observer.observe(el));
  },
}
</script>

<style>
#app {
  text-align: center;
}
body{
  background-color: #1a1a1a;
}
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
</style>
