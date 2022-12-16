<template>
  <div class="footer_wrapper">
    <div class="footer">
      © {{currentYear}} Copyright Amanda Elias 
    </div>
  </div>
</template>

<script>
export default {
  name: 'PortfolioFooter',
  props: {
    msg: String
  },
  data(){
    return{
      currentDate: null,
      currentYear: null,
    }
  },

  mounted: function(){
      this.currentDate = new Date();
      this.currentYear = this.currentDate.getFullYear();
  },
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Marcellus&family=Work+Sans:wght@300&display=swap');

.footer_wrapper{
  min-height: 100%;
  position: relative;
}
.footer{
  color: white;
  font-size: 12px;
}
</style>
