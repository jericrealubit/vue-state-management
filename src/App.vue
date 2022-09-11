<template>
  <CartCounter />
  <hr>
  <CartTotal />
</template>

<script>
import CartCounter from "./components/CartCounter.vue";
import CartTotal from "./components/CartTotal.vue";
import { provide } from "vue";
import store from "@/store";

export default {
  name: "App",
  components: {
    CartCounter,
    CartTotal
  },
  setup () {
    provide("store", store)
  }
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
