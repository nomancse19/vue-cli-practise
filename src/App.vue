<template>
  <HelloWorld msg="Welcome To My Vue Js Site"></HelloWorld>
  <Welcome />
  <new-data />
</template>
<script>
import HelloWorld from "./components/HelloWorld.vue";
import Welcome from "./components/WelCome.vue";
import NewData from "./components/NewData.vue";
export default {
  name: "App",
  components: {
    Welcome,
    HelloWorld,
    NewData,
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
