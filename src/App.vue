<template>
    <Navbar :logo="logo_src" :alt="app_name"/>
    <router-view/>
    <div id="separator" />
    <Footer />
</template>


<script>
  import Navbar from './components/Navbar.vue'
  import Footer from './components/Footer.vue'

  export default {
    components: {
      Navbar,
      Footer
    },
    data(){
      return {
        logo_src: '/img/logo.png',
        app_name: 'Make Your Burguer'
      }
    }
  }
</script>


<style>
  * {
    font-family: Helvetica, sans-serif;
    padding: 0;
    margin: 0;
    box-sizing: border-box;
  }

  .main-container {
    margin: 50px;
    height: 100vh;
  }

  h1 {
    text-align: center;
    font-size: 42px;
    margin-bottom: 30px;
    color: #222;
  }

  html {
    position: relative;
    min-height: 100%;
  }

  #separator {
    padding-top: 80px;
  }
</style>