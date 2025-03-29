<template>
  <header class="header">
    <div id="logo">FOSDEM</div>
    <div id="box">Box 79</div>
    <ul id="nav">
      <li>Video</li>
      <li>Audio</li>
      <li>Setup</li>
    </ul>
  </header>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#logo {
  font-size: 2em;
  color: rebeccapurple;
  font-weight: bold;
  line-height: 48px;
  height: 48px;
  float: left;
  padding-left: 10px;
  padding-right: 10px;
}

ul {
  display: block;
  padding: 0;
  margin: 0;
  list-style: none;
}

li {
  display: inline-block;
  height: 48px;
  line-height: 48px;
  padding-left: 10px;
  padding-right: 10px;
}

#box {
  float: right;
  height: 48px;
  line-height: 48px;
  padding-right: 10px;
}
</style>
