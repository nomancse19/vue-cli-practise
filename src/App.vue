<template>
  <HelloWorld msg="Welcome To My Vue Js Site"></HelloWorld>
  <CustomComponent
    age="27"
    name="Jahidul Islam Noman"
    department="CSE"
    skill="PHP, Laravel,Zend Certified"
  ></CustomComponent>
  <CustomComponent
    age="25"
    name="Test Purpose Name"
    department="Non CSE"
    skill="No Skills Available"
  ></CustomComponent>
</template>
<script>
import HelloWorld from "./components/HelloWorld.vue";
import CustomComponent from "./components/CustomComponent.vue";
export default {
  name: "App",
  components: {
    HelloWorld,
    CustomComponent,
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
