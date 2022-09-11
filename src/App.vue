<template>
  <HelloWorld msg="Welcome To My Vue Js Site" class="hello"></HelloWorld>
  <ApiPostData></ApiPostData>
  <product-card
    v-for="product in products"
    :key="product.name"
    :prop_product="product"
    @buy-now-click="clickBuy($event)"
    @add-to-cart="addtocart()"
  ></product-card>
</template>
<script>
import HelloWorld from "./components/HelloWorld.vue";
import ProductCard from "./components/ProductCard.vue";
import ApiPostData from "./components/ApiPostData.vue";
export default {
  name: "App",

  data() {
    return {
      products: [
        {
          name: "Apple iPhone 13 Pro Max",
          thumbnail:
            "https://fdn2.gsmarena.com/vv/bigpic/apple-iphone-13-pro-max.jpg",
          price: 99850,
        },
        {
          name: "Xiaomi Redmi 11T Pro",
          thumbnail:
            "https://fdn2.gsmarena.com/vv/bigpic/xiaomi-redmi-note-11t-pro.jpg",
          price: 55800,
        },
        {
          name: "Xiaomi Redmi 10 Prime 2022",
          thumbnail: "https://fdn2.gsmarena.com/vv/bigpic/xiaomi-redmi-10-.jpg",
          price: 32500,
        },
      ],
    };
  },
  methods: {
    clickBuy(product_name) {
      console.log(product_name.name);
    },
    addtocart() {
      console.log("Add To Cart...");
    },
  },
  components: {
    HelloWorld,
    ProductCard,
    ApiPostData,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
  text-align: center;
}
.hello {
  text-align: center;
}
button {
  padding: 5px 5px;
  margin: 5px;
  cursor: pointer;
}

.the-product__body img {
  height: 110px;
}
</style>
