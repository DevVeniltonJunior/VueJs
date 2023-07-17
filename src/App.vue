<template>

  <nav-bar :logo="logo_src" :alt="app_name"/>
  <router-view />
  <Footer />
</template>

<script>
import NavBar from './components/NavBar.vue'
import Footer from './components/Footer.vue'

export default {
  components: {
    NavBar,
    Footer
  },
  data() {
    return {
      logo_src: './img/logo.png',
      app_name: 'Make your burger'
    }
  }
}
</script>


<style>
  @import url('https://fonts.googleapis.com/css2?family=Comic+Neue&family=Inter:wght@400;500&display=swap');
  
  * {
  font-family: 'Comic Neue', cursive;
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  }

  .main-container {
    margin: 50px;
    min-height: 100vh;
  }

  h1 {
    text-align: center;
    font-size: 42;
    margin-bottom: 30px; 
    color: #222;
  }
</style>
