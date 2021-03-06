<template>
  <div class="main">
    <div class="slider">
      
      <div class="img-slider">
        <img src="@/assets/images/2.jpg" alt="">
      </div>
      <div class="img-slider">
        <img src="@/assets/images/1.jpg" alt="">
      </div>
      <div class="img-slider">
        <img src="@/assets/images/3.jpg" alt="">
      </div>
      <div class="img-slider">
        <img src="@/assets/images/4.jpg" alt="">
      </div>
      <div class="img-slider">
        <img src="@/assets/images/5.jpg" alt="">
      </div>

    </div>
  </div>
</template>

<script>
  export default {
    mounted(){
      let slider = document.querySelector('.slider')
      let s = 0
      for(let i=0; i<5; i++){
        let timerId = setInterval(() => {
          s += 100
          slider.style.transform = `translate(-${s}vw)`
        }, 3000)
      }
        setTimeout(() => {
          clearInterval(timerId);  
        }, 3000)
    }
  }
</script>

<style scoped>  
  .main{
    position: relative;
    width: 100%;
    min-height: 100vh;
    height: 100%;
    overflow: hidden;
  }
  .slider{
    position: relative;
    display: flex;
    justify-content: space-evenly;
    width: 500%;
    transition: transform 1s ease;
  }
  .img-slider{
    position: relative;
    max-height: 100vh;
    max-width: 100vw;
  }
  .img-slider img{
    width: 100%;
    height: calc(100vh);
    object-fit: cover;
    display: block;
    overflow: hidden;
  }
</style>
