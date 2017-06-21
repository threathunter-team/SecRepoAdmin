<template>
  <div id="app">
    <div class="layout">
      <sidebar></sidebar>
      <main-content></main-content>
    </div>

    <!--
    <img src="https://threathunter.org/public/images/logo_ico.png">
    <router-view></router-view>
    -->
  </div>
</template>

<script>
  import Sidebar from "./components/Sidebar";
  import MainContent from "./components/Maincontent";
  export default {
    components: {Sidebar,MainContent},
    name: 'app'
  }
</script>

<style>
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }

  .layout {
    padding-left: 160px;
    left: 0;
  }

  body {
    min-width: 320px;
    background-color: #fff;
    color: #777;
    line-height: 1.6;
  }







</style>
