<template>
  <HelloWorld msg="Welcome To My Vue Js Site"></HelloWorld>
  <PropsValidation
    v-for="contacts in ContactDetails"
    :key="contacts.name"
    :name="contacts.name"
    :skill="contacts.skill"
    :department="contacts.department"
    :age="contacts.age"
  ></PropsValidation>

  <ComponentSlot
    v-for="contacts in ContactDetails"
    :key="contacts.name"
    :name="contacts.name"
    :skill="contacts.skill"
    :department="contacts.department"
    :age="contacts.age"
  >
    <span style="color: red">Hello I AM Inside From Component Slot.... </span>
  </ComponentSlot>
</template>
<script>
import HelloWorld from "./components/HelloWorld.vue";
import PropsValidation from "./components/PropsValidation.vue";
import ComponentSlot from "./components/ComponentSlot.vue";
export default {
  name: "App",

  data() {
    return {
      ContactDetails: [
        {
          name: "Jahidul Islam Noman",
          age: 25,
          department: "CSE",
          skill: "Laravel, PHP, Jquery",
        },
        {
          name: "Jahid Khan",
          age: 15,
          department: "Class Ten",
          skill: "Asp.net, C#",
        },
      ],
    };
  },
  components: {
    HelloWorld,
    PropsValidation,
    ComponentSlot,
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
