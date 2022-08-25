<template>
  <div id="app">
    <MyHeader />
    <MyJumbotron />
    <MyMain />
    <MyFooterTop />
    <MyFooter />
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue';
import MyJumbotron from './components/MyJumbotron.vue';
import MyMain from './components/MyMain.vue';
import MyFooterTop from './components/MyFooterTop.vue';
import MyFooter from './components/MyFooter.vue';

export default {
  name: 'App',
  components: {
    MyHeader,
    MyJumbotron,
    MyMain,
    MyFooterTop,
    MyFooter
  }
}
</script>

<style lang="scss">

@import './styles/general_rules.scss';

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

</style>