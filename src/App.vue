<template>
  <div id="app">
    <Main/>
  </div>
</template>

<script>
  import Main from './components/Main'  
  export default {
    name: 'App',
    components:{
      Main  
    }
  }
</script>

<style>
  #app, *{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
</style>
