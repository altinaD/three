<template>
  <div class="main">
    <div class="img-slider">
      <img src="@/assets/2.jpg" alt="">
    </div>
  </div>
</template>

<script>
  export default {
    
  }
</script>

<style scoped>  
  .main{
    position: relative;
    width: 100%;
  }
  .img-slider{
    width: 100%;
    min-height: 100vh;  
    height: auto;
    position: relative;
  }
  .img-slider img{
    position: absolute;
    width: 100%;
    height: auto;
  }
</style>
