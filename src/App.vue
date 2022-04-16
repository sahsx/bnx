<template>
  <div id="app">
    <battle-page />
  </div>
</template>

<script>
import BattlePage from "./components/BattlePage.vue";

export default {
  name: "App",
  components: {
    BattlePage,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
