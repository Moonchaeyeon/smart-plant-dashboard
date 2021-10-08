<template>
<div class="title"></div>
<SideBar></SideBar>
<router-view></router-view>
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
  position: absolute;
  top: 0%;
  width: 250px;
  height: 1000px;
  background-color: #1a233a;
  color: #c8d9f8;
  text-align: left;
  padding: 10px;
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
