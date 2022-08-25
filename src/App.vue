<template>
  <div id="app">
    <MyHeader />
    <MyJumbotron />
    <MyProducts />
    <MyFooter />
  </div>
</template>

<script>
import MyHeader from './components/MyHeader';
import MyProducts from './components/MyProducts';
import MyFooter from './components/MyFooter';
import MyJumbotron from './components/MyJumbotron.vue';

export default {
  name: 'App',
  components: {
    MyHeader,
    MyProducts,
    MyFooter,
    MyJumbotron
  }
}
</script>

<style lang="scss">
  @import './style/vars.scss';
  @import './style/mixin.scss';
  @import './style/typo.scss';
  @import './style/utilities.scss';
  @import '~bootstrap/scss/bootstrap.scss';


  #app {
    height: 100vh;
    
  }

</style>
