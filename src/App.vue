<template>
  <el-container id="app">
    <el-aside width="300px">
      <main-nav></main-nav>
    </el-aside>
    <el-container>
      <el-main class="main">
        <router-view></router-view>
      </el-main>
      <el-footer>
        <player />
      </el-footer>
    </el-container>
  </el-container>
</template>
<script>
import nav from './components/nav';
import player from './components/player';
export default {
  name: 'app',
  components: { 'main-nav': nav, player }
};
</script>
<style>
.aside {
  background-color: azure;
}
.main {
  height: 100%;
}
html,
body,
#app {
  height: 100%;
}
body{
  margin: 0;
}
</style>
