<template>
  <div class="hello">
    <div class="pure-g">
      <div class="pure-u-1-3">
      </div>
      <div class="pure-u-1-3">
        <form class="pure-form">
          <fieldset class="pure-group">
            <input type="text" class="pure-input-1" placeholder="Username">
            <input type="password" class="pure-input-1" placeholder="Password">
          </fieldset>

          <fieldset class="pure-group">
            <input type="text" class="pure-input-1" placeholder="Verification Code">
          </fieldset>
          <button type="submit" class="pure-button pure-input-1-2 pure-button-primary">Sign in</button>
        </form>

      </div>
      <div class="pure-u-1-3">
      </div>
    </div>

  </div>
</template>

<script>
  export default {
    name: 'hello',
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .pure-group {
    width: 68%;
    margin: auto;

  }

</style>
