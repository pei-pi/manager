<template>
  <div id="app">
    <HelloWorld msg="Welcome to Your Vue.js App" />
    <el-container>
      <el-header>
        <p>LOGO</p>
      </el-header>
      <el-container class="ctr">
        <el-aside class="aside-left" width="100px">
          <el-col class="img">
            <el-avatar shape="square" :size="40"></el-avatar>
            <el-avatar shape="square" :size="40"></el-avatar>
            <el-avatar shape="square" :size="40"></el-avatar>
            <el-avatar shape="square" :size="40"></el-avatar>
          </el-col>
        </el-aside>
        <el-aside class="aside-right" width="200px">
          <el-col>
            <el-menu default-active="2" class="el-menu-vertical-demo">
              <el-menu-item index="1">
                <span slot="title">二级导航</span>
              </el-menu-item>
              <el-menu-item index="2">
                <span slot="title">二级导航</span>
              </el-menu-item>
              <el-menu-item index="3">
                <span slot="title">二级导航</span>
              </el-menu-item>
              <el-menu-item index="4">
                <span slot="title">二级导航</span>
              </el-menu-item>
            </el-menu>
          </el-col>
        </el-aside>
        <el-main></el-main>
      </el-container>
    </el-container>
    <div class="clear"></div>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
  },
};
</script>

<style>
.clear {
  clear: both;
}
body {
  margin: 10px;
  background-color: #f9fafc;
}
#app {
  background-color: #e5e9f2;
  width: 100%;
  border-radius: 10px;
}
/* 头部 */
.el-header {
  background-color: #324057;
  color: #f9fafc;
  border-radius: 10px 10px 0 0;
}
p {
  font-size: 25px;
  font-weight: 500;
  line-height: 17px;
  float: left;
  margin-left: 30px;
}
/* 主体部分 */
.ctr {
  height: 500px;
}
.el-aside {
  background-color: white;
  color: #333;
  text-align: center;
  line-height: 200px;
}
.el-main {
  background-color: #e9eef3;
  color: #333;
  text-align: center;
  line-height: 160px;
}
body > .el-container {
  margin-bottom: 40px;
}
/* 左 */
.aside-left {
  margin-right: 5px;
  border-radius: 0 0 0 10px;
}
.img {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
.el-avatar {
  margin-top: 20px;
}
/* 右 */
.el-main {
  background-color: white;
  margin: 20px;
}
</style>
