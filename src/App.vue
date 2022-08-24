<template>
  <div id="app">
    <MyHeader />
    <MyProducts />
    <MyFooter />
  </div>
</template>

<script>
import MyHeader from './components/MyHeader';
import MyProducts from './components/MyProducts';
import MyFooter from './components/MyFooter';

export default {
  name: 'App',
  components: {
    MyHeader,
    MyProducts,
    MyFooter
}
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
