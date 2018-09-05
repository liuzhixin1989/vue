<template>
  <div class="confirm-button">
      <button @click="getButtonCLick">{{text||'确认'}}</button>
  </div>
</template>

<script>
export default {
  name: 'confirm-button',
  props:['text'],//父组件穿给子组件的值
  data () {
    return {
      msg: 'true'
    }
  },
  methods:{
      getButtonClick(){ //点击按钮的时候，向父组件传值
          this.$emit("message",this.msg);//向父组件传值
      }/*父组件传给子组件的值通过proos接收，子组件通过$emit向父组件传值 */
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    .confirm-button{
        height:40px;
        line-height: 40px;
    }
    button{
        width: 60px;
        height: 26px;
        color:#42b983;
        border: solid 1px currentColor;
        background-color: #fff;
    }
</style>
