<template>
  <div>
    <!-- <h1>Vuex: Beginners</h1>
    <ul v-for="product in products" :key="products.indexOf(product.name)">
      <li>{{ product.name }}</li>
    </ul> -->
    <ProductOne v-bind:products="products" />
    <ProductTwo v-bind:products="products" />
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
    return {
      products: [
        { name: "Banana Skin", price: 20 },
        { name: "Skinny Star", price: 40 },
        { name: "Green Shells", price: 60 },
        { name: "Red Shells", price: 80 },
      ],
    };
  },
};
</script>

<style>
body {
  font-family: Ubuntu;
  color: #555;
}
</style>
