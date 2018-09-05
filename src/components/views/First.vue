<template>
  <div class="first-app">
    <h1>{{ msg }}</h1>
    <router-link to="Second">第二个页面</router-link>
    <Confirm text="注册" @message="getMeaasge"></Confirm>
  </div>
</template>

<script>
import Confirm from '../sub/Confirm'
export default{
  name:'First',
  components:{
    Confirm
  },
  data(){
    return {
      msg:'welcome to First views'
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
<style scoped>
h1, h2 {
  font-weight: normal;
}
a {
  color: #42b983;
}
</style>
