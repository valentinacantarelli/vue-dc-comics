<template>
  <div id="app">
    <Header/>
    <main>
      <Hero :bgImg="require('./assets/img/jumbotron.jpg')"/>
      <MainSection/>
      <BannerIcons/>
    </main>
    <Footer/>
  </div>
</template>

<script>
import BannerIcons from './components/BannerIcons.vue'
import Footer from './components/Footer.vue'
import Header from './components/Header.vue'
import MainSection from './components/MainSection.vue'
import Hero from './components/Hero.vue'

export default {
  name: 'App',
  components: {
    BannerIcons,
    Footer,
    Header,
    MainSection,
    Hero
  }
}
</script>

<style lang="scss">
@import "./assets/style/common";


</style>
