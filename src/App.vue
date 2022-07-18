<template>
  <div id="app">
    <headerMain/>
    <mainContent/>
    <shopperContent/>
    <mainNews/>
    <footerMain/>
  </div>
</template>

<script>
import headerMain from './components/header.vue'
import mainContent from './components/main.vue'
import shopperContent from './components/shopper.vue'
import footerMain from './components/footer.vue'
import mainNews from './/components/mainNews.vue'

export default {
  name: 'App',
  components: {
    headerMain ,
    mainContent,
    shopperContent,
    footerMain,
    mainNews
  }
}
</script>

<style lang="scss">
@import "~/node_modules/bootstrap/scss/bootstrap.scss";
@import "./styles/variables.scss";
@import "./styles/general.scss";




</style>
