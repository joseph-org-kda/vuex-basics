<template>
  <div>
    <!-- <h1>Vuex: Beginners</h1>
    <ul v-for="product in products" :key="products.indexOf(product.name)">
      <li>{{ product.name }}</li>
    </ul> -->
    <ProductOne :products="products" />
    <ProductTwo :products="products" />
  </div>
</template>

<script>
import ProductOne from "./components/ProductOne.vue";
import ProductTwo from "./components/ProductTwo.vue";

export default {
  name: "App",
  components: {
    ProductOne,
    ProductTwo,
  },
  data() {
    return {};
  },
};
</script>

<style>
body {
  font-family: Ubuntu;
  color: #555;
}
</style>
