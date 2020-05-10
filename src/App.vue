<template>
  <div id="app">
    <TopMenu/>
    <Content/>
    <Footer/>
  </div>
</template>

<script>
import TopMenu from './components/TopMenu.vue'
import Content from './components/Content.vue'
import Footer from './components/Footer.vue'


export default {
  name: 'App',
  components: {
    TopMenu,
    Content,
    Footer
  }
}
</script>

<style>
  html{
        scroll-behavior: smooth;
  }
  @font-face {
    font-family: 'EBGaramond';
    src: url('~@/assets/fonts/EBGaramond-VariableFont_wght.ttf');
    font-family: 'Roboto';
    src: url('~@/assets/fonts/Roboto-Regular.ttf');
    font-family: 'FiraSansCondensed';
    src: url('~@/assets/fonts/FiraSansCondensed-Light.ttf');
  }
  #app {
    font-family: Roboto, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    background-color: #0f38ab;
  }
</style>
