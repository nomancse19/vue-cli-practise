<template>
  <HelloWorld msg="Welcome To My Vue Js Site"></HelloWorld>
  <Welcome />
  <Welcome />
</template>
<script>
import HelloWorld from "./components/HelloWorld.vue";
import Welcome from "./components/WelCome.vue";
export default {
  name: "App",
  components: {
    Welcome,
    HelloWorld,
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
