<template>
  <HelloWorld msg="Welcome To My Vue Js Site"></HelloWorld>
  <the-card demo_title="Apple iPhone 13">
    <img src="https://fdn2.gsmarena.com/vv/bigpic/apple-iphone-13.jpg" alt="" />
    <p>
      DISPLAY Type Super Retina XDR OLED, HDR10, Dolby Vision, 800 nits (HBM),
      1200 nits (peak) Size 6.1 inches, 90.2 cm2 (~86.0% screen-to-body ratio)
      Resolution 1170 x 2532 pixels, 19.5:9 ratio (~460 ppi density)
    </p>
  </the-card>
  <the-card demo_title="Samsung Galaxy Tab Active4 Pro">
    <img
      src="https://fdn2.gsmarena.com/vv/bigpic/samsung-galaxy-a13-a137.jpg"
      alt=""
    />
    <p>
      DISPLAY Type TFT LCD Size 10.1 inches, 295.8 cm2 (~71.5% screen-to-body
      ratio) Resolution 1920 x 1200 pixels, 16:10 ratio (~224 ppi density)
    </p>
  </the-card>
  <the-card demo_title="About Services">
    <ul>
      <li>Web Development</li>
      <li>Android App</li>
      <li>Web Design</li>
      <li>Seo & Affriate</li>
      <li>Digital Marketing</li>
    </ul>
  </the-card>
</template>
<script>
import HelloWorld from "./components/HelloWorld.vue";
import TheCard from "./components/TheCard.vue";
export default {
  name: "App",

  data() {
    return {};
  },
  components: {
    HelloWorld,
    TheCard,
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
