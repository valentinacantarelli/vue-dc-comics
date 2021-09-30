<template>
  <div id="app">
    <Header/>
    <main>
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
// #app{
//   width:65%;
//   margin: auto;
// }
main{
  
  display:flex;
}
</style>
