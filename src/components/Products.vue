<template>
  <div class="main">
    <ul>
      <li v-for="product in allProducts" :key="product.id">
        {{ product.price }} | {{ product.title }}
      </li>
    </ul>
  </div>
</template>

<script>
import { mapGetters } from "vuex";
export default {
  name: "Products",
  computed: mapGetters(["allProducts"]),
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
