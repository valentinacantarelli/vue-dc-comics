<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
import BannerIcons from './components/BannerIcons.vue'
import Footer from './components/Footer.vue'
import Header from './components/Header.vue'
import MainSection from './components/MainSection.vue'

export default {
  name: 'App',
  components: {
    BannerIcons,
    Footer,
    Header,
    MainSection
  }
}
</script>

<style lang="scss">
@import "./assets/style/common";
#app {
  
}
</style>
