<template>
  <div id="app">
    <sidebar />
    <main-section />
  </div>
</template>

<script>
import Sidebar from "./components/Sidebar.vue";
import MainSection from "./components/Main.vue";
export default {
  name: "app",
  components: { Sidebar, MainSection }
};
</script>

<style lang="scss">
body {
  margin: 0;
}

#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  display: grid;
  grid-template-columns: 180px 1fr;
  grid-template-rows: 1fr;
  height: 100vh;
}
</style>
