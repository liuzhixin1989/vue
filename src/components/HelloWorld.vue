<template>
  <div class="hello">
    <div class="header">
      <div class="dq">赣州<i class="el-icon-arrow-down"></i></div>
      <div class="search">
        <i class="el-icon-search"></i>
        <input type="text" v-model="input" placeholder="输入上家/类品/商圈"></input>
      </div>
      <div class="gr">
        <a href="javascript:void(0);">
          <i class="iconfont icon-wo"></i>
          <br>
        我的
        </a>
      </div>
    </div>
    <div class="main">
      <div class="tit">
        <img src="./../assets/img/download_banner.png" alt="">
        <a href="javascript:void(0);" class="openApp"></a>
        <a href="javascript:void(0);" class="downApp"></a>
      </div>
      <div class="otherList">
        <ul>
          <li>
            <a href="javascript:void(0);">
              <span class="iconfont icon-meishi iimg"></span>
              <span>美食</span>
            </a>
          </li>
          <li>
            <a href="javascript:void(0);">
              <span class="iconfont icon-mao iimg"></span>
              <span>猫眼电影</span>
            </a>
          </li>
          <li>
            <a href="javascript:void(0);">
              <span class="iconfont icon-jiudian iimg"></span>
              <span>美食</span>
            </a>
          </li>
          <li>
            <a href="javascript:void(0);">
              <span class="iconfont icon-xiuxianyule iimg"></span>
              <span>美食</span>
            </a>
          </li>
          <li>
            <a href="javascript:void(0);">
              <span class="iconfont icon-icon-test iimg"></span>
              <span>美食</span>
            </a>
          </li>
          <li>
            <a href="javascript:void(0);">
              <span class="iconfont icon-baoji iimg"></span>
              <span>美食</span>
            </a>
          </li>
          <li>
            <a href="javascript:void(0);">
              <span class="iconfont icon-zhoubianyou iimg"></span>
              <span>美食</span>
            </a>
          </li>
          <li>
            <a href="javascript:void(0);">
              <span class="iconfont icon-liren iimg"></span>
              <span>美食</span>
            </a>
          </li>
          <li>
            <a href="javascript:void(0);">
              <span class="iconfont icon-xiaochikuaican iimg"></span>
              <span>美食</span>
            </a>
          </li>
          <li>
            <a href="javascript:void(0);">
              <span class="iconfont icon-quanbufenlei iimg"></span>
              <span>美食</span>
            </a>
          </li>
        </ul>
      </div>
      <p><router-link to="/First">去第一个页面</router-link></p>
      </div>
    <div class="footer">底部</div>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data() {
    return {
      msg: "Welcome to Your Vue.js App",
      input: ""
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="less" scoped>
body {
  margin: 0;
  background-color: rgb(240, 239, 237);
}
.header {
  height: 40px;
  display: flex;
  align-items: center;
  background-color: rgb(6, 193, 174);
  .dq {
    width: 16vw;
    color: #fff;
  }
  .search {
    width: 70vw;
    background-color: rgb(5, 164, 148);
    border-radius: 5px;
    height: 30px;
    input {
      width: 80%;
      background-color: rgb(5, 164, 148);
      outline: none;
    }
    i {
      color: #fff;
    }
  }
  .gr {
    width: 14vw;
    a {
      display: block;
      width: 100%;
      color: #fff;
      font-size: 12px;
      height: 40px;
    }
    i {
      font-size: 22px;
    }
  }
}
.main {
  width: 100vw;
  height: auto;
  .tit {
    width: 100vw;
    height: auto;
    position: relative;
    img {
      width: 100%;
    }
    a {
      position: absolute;
      display: block;
      width: 31%;
      height: 34%;
      z-index: 1;
    }
    .openApp {
      left: 17%;
      bottom: 12%;
    }
    .downApp {
      right: 17%;
      bottom: 12%;
    }
  }
  .otherList{
    height: 3.3rem;
    border-top:solid 1px #ccc;
    ul{
       height: 7.3rem;
      li{
        height: 50%;
        width: 20vw;
        text-align: center;
        float: left;
        a{
          display: block;
          padding: 0.5rem 0;
        }
        .iimg{
          display: block;
          font-size: 18px;
          height: 1.8rem;
          width: 1.8rem;
          line-height: 1.8rem;
          margin: 0 auto;
          border-radius: 50%;
          color: #fff;
          background-color: #fd9d21;
        }
        span{
          font-size: 12px;
          color: #333;
        }
      }
      li:nth-child(2) a .iimg{
        background-color: #ff6767;
      }
      li:nth-child(3) a .iimg{
        background-color: #8a90fa;
      }
      li:nth-child(4) a .iimg{
        background-color: #fed030;
      }
      li:nth-child(5) a .iimg{
        background-color: #fd9d21;
      }
      li:nth-child(6) a .iimg{
        background-color: #fed030;
      }
      li:nth-child(7) a .iimg{
        background-color: #4dc6ee;
      }
      li:nth-child(8) a .iimg{
        background-color: #ff80c2;
      }
      li:nth-child(9) a .iimg{
        background-color: #fd9d21;
      }
      li:nth-child(10) a .iimg{
        background-color: #00d3be;
      }
    }
  }
}
h1,
h2 {
  font-weight: normal;
  margin: 0;
}
a {
  color: #42b983;
}
</style>
