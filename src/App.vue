<template>
  <div id="app">
    <!--<navbar :signin="signedinOrNot"/>-->
    <navbar/>
    <router-view/>
    <footerNav/>
    <uparrow/>
  </div>
</template>

<script>
import navbar from "./components/navbar"
import footerNav from "./components/footerNav"
import uparrow from "./components/smallcomponents/topbutton"

export default {
  name: 'App',
  /*data: ()=> ({
    signedinOrNot: false
  }),*/
  components: { navbar, footerNav, uparrow }
}
</script>

<style>
  body{
    margin: 0 auto;
    background-color: #e6e6e6;
  }
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    /*text-align: center;*/ /*það þarf að centera textan annarstaðar.*/
    color: #2c3e50;
  }
</style>
