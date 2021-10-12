<template>
<div style="display: flex; flex-direction: row;">
  <SideBar></SideBar>
  <div style="width:100%;">
    <div class="title"></div>
    <router-view></router-view>
  </div>
</div>
<div class="footer">경희대학교</div>
</template>

<script>
import SideBar from "./components/SideBar.vue"; 
export default {
  name: 'App',
  components: {
    SideBar: SideBar,
  }
}
</script>

<style>
.title {
  width: 100%;
  height: 60px;
  background-color: #1a233a;
}
.side-bar {
  width: 300px;
  height: 100%;
  background-color: #1a233a;
  color: #c8d9f8;
  text-align: left;
  padding: 10px;
  box-shadow: 1px 0px 10px 3px grey;
}

.footer {
  width:100%;
  height: 60px;
}

.menu1 {
  color: aqua;
  padding-left: 20px;
}

.menu2 {
  margin: 20px;
  padding-left: 20px;
  padding-bottom: 10px;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;

}
</style>
