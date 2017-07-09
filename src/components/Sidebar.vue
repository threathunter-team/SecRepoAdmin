<template>
  <div id="menu">
    <div class="pure-menu">
      <a class="pure-menu-heading" href="/">SecRepo</a>
      <ul class="pure-menu-list">
        <li class="pure-menu-item">
          <a href="/start/" class="pure-menu-link">控制台</a>
        </li>
        <li class="pure-menu-item">
          <a href="/layouts/" class="pure-menu-link">用户管理</a>
        </li>
        <li class="pure-menu-item">
          <a href="/layouts/" class="pure-menu-link">待审列表</a>
        </li>
        <li class="pure-menu-item menu-item-divided">
          <a href="/base/" class="pure-menu-link">源管理</a>
        </li>
        <li class="pure-menu-item pure-menu-selected">
          <a href="/grids/" class="pure-menu-link">分类管理</a>
        </li>
        <li class="pure-menu-item">
          <a href="/forms/" class="pure-menu-link">标签管理</a>
        </li>
        <li class="pure-menu-item menu-item-divided">
          <a href="#" class="pure-menu-link pure-menu-disabled">Version 1.0</a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'sidebar',
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  #menu,
  .menu-link {
    -webkit-transition: all 0.2s ease-out;
    -moz-transition: all 0.2s ease-out;
    -ms-transition: all 0.2s ease-out;
    -o-transition: all 0.2s ease-out;
    transition: all 0.2s ease-out;
  }

  #layout.active .menu-link {
    left: 160px;
  }

  #menu {
    margin-left: -160px; /* "#menu" width */
    width: 160px;
    position: fixed;
    top: 0;
    left: 0;
    bottom: 0;
    z-index: 1000; /* so the menu or its navicon stays above all content */
    background: #191818;
    overflow-y: auto;
    -webkit-overflow-scrolling: touch;
  }
  #menu a {
    color: #999;
    border: none;
    white-space: normal;
    padding: 0.625em 1em;
  }

  #menu .pure-menu-open {
    background: transparent;
    border: 0;
  }

  #menu .pure-menu ul {
    border: none;
    background: transparent;
    display: block;
  }

  #menu .pure-menu ul,
  #menu .pure-menu .menu-item-divided {
    border-top: 1px solid #333;
  }

  #menu .pure-menu li a:hover,
  #menu .pure-menu li a:focus {
    background: #333;
  }

  .menu-link {
    position: fixed;
    display: block; /* show this only on small screens */
    top: 0;
    left: 0; /* "#menu width" */
    background: #000;
    background: rgba(0,0,0,0.7);
    font-size: 11px; /* change this value to increase/decrease button size */
    z-index: 10;
    width: 4em;
    height: 4em;
    padding: 1em;
  }

  .menu-link:hover,
  .menu-link:focus {
    background: #000;
  }

  .menu-link span {
    position: relative;
    display: block;
    margin-top: 0.9em;
  }

  .menu-link span,
  .menu-link span:before,
  .menu-link span:after {
    background-color: #fff;
    width: 100%;
    height: .2em;
    -webkit-transition: all 0.4s;
    -moz-transition: all 0.4s;
    -ms-transition: all 0.4s;
    -o-transition: all 0.4s;
    transition: all 0.4s;
  }

  .menu-link span:before,
  .menu-link span:after {
    position: absolute;
    top: -.55em;
    content: " ";
  }

  .menu-link span:after {
    top: .55em;
  }

  .menu-link.active span {
    background: transparent;
  }

  .menu-link.active span:before {
    -webkit-transform: rotate(45deg) translate(.5em, .4em);
    -moz-transform: rotate(45deg) translate(.5em, .4em);
    -ms-transform: rotate(45deg) translate(.5em, .4em);
    -o-transform: rotate(45deg) translate(.5em, .4em);
    transform: rotate(45deg) translate(.5em, .4em);
  }

  .menu-link.active span:after {
    -webkit-transform: rotate(-45deg) translate(.4em, -.3em);
    -moz-transform: rotate(-45deg) translate(.4em, -.3em);
    -ms-transform: rotate(-45deg) translate(.4em, -.3em);
    -o-transform: rotate(-45deg) translate(.4em, -.3em);
    transform: rotate(-45deg) translate(.4em, -.3em);
  }

  #menu .pure-menu-heading {
    font-size: 125%;
    font-weight: 300;
    letter-spacing: 0.1em;
    color: #fff;
    margin-top: 0;
    padding: 0.5em 0.8em;
    text-transform: uppercase;
  }
  #menu .pure-menu-heading:hover,
  #menu .pure-menu-heading:focus {
    color: #999;
  }

  #menu .pure-menu-selected {
    background: #1f8dd6;
  }

  #menu .pure-menu-selected a {
    color: #fff;
  }

  #menu li.pure-menu-selected a:hover,
  #menu li.pure-menu-selected a:focus {
    background: none;
  }


  @media (min-width: 58em) {

    #layout {
      padding-left: 160px; /* left col width "#menu" */
      left: 0;
    }
    #menu {
      left: 160px;
    }
    .menu-link {
      position: fixed;
      left: 160px;
      display: none;
    }
    #layout.active .menu-link {
      left: 160px;
    }

  }
</style>
