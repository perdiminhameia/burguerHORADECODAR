<template>
  <Navbar :logo="logo_src" :alt="app_name"/>
  <RouterView/>
  <Rodape />
</template>
<script>
import Navbar from './components/Navbar.vue';
import Rodape from './components/Rodape.vue';

export default {
  components: {
    Navbar,
    Rodape
  },
  data () {
    return {
    logo_src: "/img/logo.png",
    app_name: "MAKE YOUR BURGUER"
    }
  }
}
</script>

<style>
  * {
    font-family: Helvetica;
    padding: 0;
    margin: 0;
    box-sizing: border-box;
  }
  .main-container {
    margin: 50px;
    min-height: 250px;
  }
  h1 {
    text-align: center;
    font-size: 42px;
    margin-bottom: 30px;
    color: #222;
  }
</style>

