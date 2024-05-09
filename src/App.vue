<template>
  <head>
    <meta charset="utf-8" >
      <title></title>
      <link rel="preconnect" href="https://fonts.googleapis.com">
      <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
      <link href="https://fonts.googleapis.com/css2?family=Limelight&display=swap" rel="stylesheet">
  </head>
  <div id="app">
    <log_page />
  </div>
</template>

<script>
  import log_page from './components/log_page' 
  //import reg_page from './components/reg_page'
  //import main_page from './components/main_page'

  
  export default {
  name: 'App',
  components: {
      log_page,
      //reg_page,
      //main_page
  }
}
</script>



<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
body {
  margin: 0;
}
</style>
