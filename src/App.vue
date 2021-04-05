<template>
  <div id="app">
    <Navbar />
    <Header />
    <PriceQuoteForm msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
import PriceQuoteForm from './components/PriceQuoteForm.vue';
import Header from './components/Header.vue';
import Navbar from './components/common/TheNavbar.vue';

export default {
  name: 'App',
  components: {
    Navbar,
    Header,
    PriceQuoteForm,
  },
};
</script>

<style lang="scss">
#app {
  font-family: 'Lato',Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

body {
  background: linear-gradient(170deg, #4957d1 60%, #fe0000 60%);
  background-size: auto 100%;
  background-repeat: no-repeat;
  padding-bottom: 2.5rem;
}
</style>
