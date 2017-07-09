<template>
  <div id="main">

    <div class="header">
      <h1>分类管理</h1>
      <h2>分类总量：10</h2>
    </div>
    <div class="content">
      <div class="qtable">
        <table class="pure-table pure-table-horizontal">
          <thead>
          <tr>
            <th>#</th>
            <th>分类名称</th>
            <th>备注</th>
            <th>操作</th>
          </tr>
          </thead>

          <tbody>
          <tr>
            <td>1</td>
            <td>分类名称</td>
            <td>分类说明..分类说明..分类说明..分类说明..分类说明..分.</td>
            <td>
              <a class="pure-button" href="#">修改</a>
              <a class="pure-button" href="#">删除</a>
            </td>
          </tr>
          </tbody>
        </table>
      </div>
      <div class="qform">
        <form class="pure-form">
          <fieldset>
            <legend>添加分类</legend>

            <input type="text" placeholder="分类名称...">
            <input type="text" placeholder="分类说明...">
            <button type="submit" class="pure-button pure-button-primary">提交</button>
          </fieldset>
        </form>
      </div>
    </div>
  </div>

</template>

<script>
  export default {
    name: 'catalogs',
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

  .content {
    margin-left: auto;
    margin-right: auto;
    padding-left: 1em;
    padding-right: 1em;
    max-width: 768px;
  }

  .qtable {
    padding-left: 1rem;
    margin-top: 2rem;
    margin-bottom: 2rem;
  }

</style>
