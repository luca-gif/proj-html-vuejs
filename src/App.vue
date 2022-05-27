<template>
  <div id="app">

    <HeaderComp />
    <WelcomeComponent />
    <MainComp />
    <FooterComp />

  </div>
</template>

<script>
import HeaderComp from './components/HeaderComp.vue';
import MainComp from './components/MainComp.vue';
import FooterComp from './components/FooterComp.vue';
import WelcomeComponent from './components/WelcomeComponent.vue';



export default {
  name: 'App',
  components: {
    HeaderComp,
    MainComp,
    FooterComp,
    WelcomeComponent
}
}
</script>

<style lang="scss">
@import './assets/style/_global';
@import './assets/style/_utils';
@import './assets/style/_var';



</style>
