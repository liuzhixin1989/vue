<template>
  <div class="second-app">
    <h1>{{ msg }}</h1>
    <Confirm text="注册" @message="getMeaasge"></Confirm>
    <router-link to="/" class="">首页</router-link>
  </div>
</template>

<script>
import Confirm from '../sub/Confirm'
export default{
  name:'Second',
  components:{
    Confirm
  },
  data(){
    return {
      msg:'welcome to Second views'
    }
  },
  methods:{
    getMeaasge(val){//val为子组件传个父组件的值
      alert(val)
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="less" scoped>
h1, h2 {
  font-weight: normal;
}
a {
  color: #42b983;
  font-size: 18px;
  text-decoration:none;
}
</style>
