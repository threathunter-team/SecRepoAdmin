<template>
  <div id="app">
    <div class="layout">
      <router-view></router-view>
    </div>
  </div>
</template>

<script>
  import Sidebar from "./components/Sidebar";
  import MainContent from "./components/Maincontent";
  import Users from "./components/Users";
  import AuditList from "./components/Audits";
  import RepoList from "./components/Repos";
  import CatalogList from "./components/Catalogs";
  import TagList from "./components/Tags"
  export default {
    components: {
      Users,
      Sidebar,
      MainContent,
      AuditList,
      RepoList,
      CatalogList,
      TagList
    },
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
    /* padding-left: 160px; */
    left: 0;
  }

  body {
    min-width: 320px;
    background-color: #fff;
    color: #777;
    line-height: 1.6;
  }







</style>
