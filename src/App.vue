<template>
  <div id="app">
    <el-container>
      <el-header>
        <p>LOGO</p>
      </el-header>
      <el-container>
        <el-aside>
            <el-menu class="el-menu-vertical-demo">
              <el-submenu index="1" min-width="150px">
                <template slot="title">
                  <span>
                    <el-avatar shape="square" :size="40"></el-avatar>
                  </span>
                </template>
                <el-menu-item-group>
                  <router-link to="one"><el-menu-item index="1-1">二级菜单1</el-menu-item></router-link>
                  <router-link to="two"><el-menu-item index="1-2">二级菜单2</el-menu-item></router-link>
                  <router-link to="three"><el-menu-item index="1-3">二级菜单3</el-menu-item></router-link>
                  <router-link to="four"><el-menu-item index="1-4">二级菜单4</el-menu-item></router-link>
                </el-menu-item-group>
              </el-submenu>
              <el-menu-item index="2">
                <span>
                  <el-avatar shape="square" :size="40"></el-avatar>
                </span>
              </el-menu-item>
              <el-menu-item index="3">
                <span>
                  <el-avatar shape="square" :size="40"></el-avatar>
                </span>
              </el-menu-item>
              <el-menu-item index="4">
                <span>
                  <el-avatar shape="square" :size="40"></el-avatar>
                </span>
              </el-menu-item>
            </el-menu>
        </el-aside>
        <el-main>
          <router-view></router-view>
        </el-main>
      </el-container>
    </el-container>
  </div>
</template>

<script>
export default {};
</script>
 
<style>
/* body */
body {
  margin: 10px;
  background-color: #f9fafc;
}
#app {
  background-color: #e5e9f2;
  width: 100%;
  border-radius: 10px;
  height: 500px;
  overflow: hidden;
}
/* header*/
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
/* aside */
.el-aside {
  background-color: #e5e9f2;
  color: #333;
  text-align: center;
  line-height: 200px;
  overflow: hidden;
  width: 280px;
}
.el-menu{
  width: 90px;
  position:absolute;
  height:440px;
  border-radius: 0 0 0 10px;
}
li{
  height: 56px;
}
.el-menu-item-group>ul{
  position: relative;
  left: 100px;
  top: -70px;
  background-color: white;
  height: 440px;
  width: 200px;
  min-width: 0;
  overflow: hidden;
}
a{
  text-decoration: none;
  color:black;
}
/* 小箭头隐藏 */
.el-submenu__icon-arrow::before{
  display: none;
}
/* main */
.el-main{
  padding: 0px;
}
</style>
