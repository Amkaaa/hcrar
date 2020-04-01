<template>
  <div id="app">
    <Header/>
    <router-view/>
    <Footer/>
  </div>
</template>

<script>
import Header from './components/layout/Header';
import Footer from './components/layout/Footer';

export default {
  components: {
    Header,
    Footer
  }
}
</script>

<style>
  html {
    scroll-behavior: smooth;
  }
  body{
    margin: 0;
    padding: 0;
  }

</style>
