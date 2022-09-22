<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <HelloWorld msg="Welcome to Your Vue.js App" />
  <Posts msg="howdy!" />
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import Posts from "./components/Posts.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
    Posts,
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
