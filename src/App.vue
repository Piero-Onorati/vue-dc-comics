<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <Header/>
    <!-- <MainContent/>
    <HighlightedContent/>
    <Footer/>
    <CTASocial/>   -->
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import Header from './components/Header.vue'
// import MainContent from './components/MainContent.vue'
// import HighlightedContent from './components/HighlightedContent.vue'
// import Footer from './components/Footer.vue'
// import CTASocial from './components/CTASocial.vue'


export default {
  name: 'App',
  components: {
    // HelloWorld
    Header,
    // MainContent,
    // HighlightedContent,
    // Footer,
    // CTASocial
  }
}
</script>

<style lang="scss">
@import 'style/commons.scss';

</style>
