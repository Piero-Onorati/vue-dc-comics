<template>
  <div id="app">
    <Header/>
    <MainContent/>
    <HighlightedContent/>
    <Footer/>
    <CTASocial/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import MainContent from './components/MainContent.vue'
import HighlightedContent from './components/HighlightedContent.vue'
import Footer from './components/Footer.vue'
import CTASocial from './components/CTASocial.vue'

export default {
  name: 'App',
  components: {
    Header,
    MainContent,
    HighlightedContent,
    Footer,
    CTASocial
  }
}
</script>

<style lang="scss">
@import 'style/commons.scss';

</style>
