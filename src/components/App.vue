<template>
  <div id="app">
    <img width="25%" src="./assets/logo.png">
    <Counter />
    <TSCounter />
  </div>
</template>

<script>
import Counter from "./components/Counter.vue";
import TSCounter from "./components/TSCounter.vue";

export default {
  name: "App",
  components: {
    Counter, TSCounter
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

