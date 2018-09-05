<template>
  <div class="hello">
    <el-header><h1>{{ msg }}</h1></el-header>
    <el-main><p><router-link to="/First">去第一个页面</router-link></p></el-main>
    <el-footer>底部</el-footer>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
body{
  margin: 0;
}
h1, h2 {
  font-weight: normal;
  margin: 0;
}
a {
  color: #42b983;
}
</style>
