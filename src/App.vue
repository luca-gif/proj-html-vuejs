<template>
  <div id="app">

    <HeaderComp :headerList="myHeader" />

    <MainComp />

    <FooterComp :footerList="myFooter" />

  </div>
</template>

<script>
import HeaderComp from './components/HeaderComp.vue';
import MainComp from './components/MainComp.vue';
import FooterComp from './components/FooterComp.vue';

import headerList from './assets/json/headerList'
import footerList from './assets/json/footerList'


export default {
  name: 'App',
  data() {
    return {
      myHeader: headerList,
      myFooter: footerList,
    }
  },
  components: {
    HeaderComp,
    MainComp,
    FooterComp,
  }
}
</script>

<style lang="scss">
@import './assets/style/_global';
@import './assets/style/_utils';
@import './assets/style/_var';
</style>
