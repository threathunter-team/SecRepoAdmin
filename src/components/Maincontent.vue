<template>
  <div id="main">

    <div class="header">
      <h1>控制台</h1>
      <h2>最后更新时间 2017-06-21 17:07</h2>
    </div>
    <div class="content">

    </div>
  </div>

</template>

<script>
  export default {
    name: 'maincontent',
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

  .header {
    max-width: 768px;
    margin: 0 auto;
    padding: 1em;
    text-align: center;
    border-bottom: 1px solid #eee;
    background: #fff;
    letter-spacing: 0.05em;
  }

  .header h1 {
    font-size: 320%;
    font-weight: 100;
    margin: 0;
  }

  .header h2 {
    font-size: 128%;
    font-weight: 100;
    line-height: 1.5;
    margin: 0;
    color: #666;
    letter-spacing: -0.02em;
  }

</style>
