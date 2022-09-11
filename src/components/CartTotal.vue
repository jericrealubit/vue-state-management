<template>
  <h2>Cart Total</h2>
  <div class="counter">{{ store.state.counter }}</div>
</template>

<script>
import { inject } from "vue";
export default {
  name: "cart-total",
  setup() {
    const store = inject("store")

    return {
      store
    };
  },
};
</script>

<style>
</style>
