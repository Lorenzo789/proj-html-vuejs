<template>
  <div id="app">
    <!-- 26/07/22 FINIRE HEADER E MINIMO UN PEZZO MAIN CSS INCLUSO -->
    <Header />

    <Main />

    <Footer />
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Main from './components/Main.vue';
import Footer from './components/Footer.vue';


export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer
  },
  data: function(){
    return{

    }
  }
}
</script>

<style lang="scss">
@import'../node_modules/bootstrap/dist/css/bootstrap.css';

</style>
