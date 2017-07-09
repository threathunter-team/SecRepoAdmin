<template>
  <div id="main">

    <div class="header">
      <h1>源管理</h1>
      <h2>源总量：60</h2>
    </div>
    <div class="content">
      <div class="qtable">
        <table class="pure-table pure-table-horizontal">
          <thead>
          <tr>
            <th>#</th>
            <th>提交用户</th>
            <th>项目地址</th>
            <th>操作</th>
          </tr>
          </thead>

          <tbody>
          <tr>
            <th><input type="checkbox"> </th>
            <td>feixin</td>
            <td><a href="#">https://github.com/rapid7/metasploit-framework</a></td>
            <td>
              <a class="pure-button" href="#">详情</a>
              <a class="pure-button" href="#">审核</a>
              <a class="pure-button" href="#">修改</a>
              <a class="pure-button" href="#">删除</a>
            </td>
          </tr>
          </tbody>
        </table>
      </div>
    </div>
  </div>

</template>

<script>
  export default {
    name: 'repos',
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

  .header {
    max-width: 1024px;
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

  .content {
    margin-left: auto;
    margin-right: auto;
    padding-left: 1em;
    padding-right: 1em;
    max-width: 1024px;
  }

  .qtable {
    padding-left: 1rem;
    margin-top: 2rem;
    margin-bottom: 2rem;
  }

</style>
