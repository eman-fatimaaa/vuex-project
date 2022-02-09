<template>
  <div class="main">
    <ul>
      <li v-for="product in allProducts" :key="product.id">
        {{ product.price | currency }} | {{ product.title }}
      </li>
    </ul>
  </div>
</template>

<script>
import { mapGetters, mapActions } from "vuex";
export default {
  name: "Products",
  created() {
    this.getProducts();
  },
  filters: {
    currency: function (value) {
      return " $" + parseFloat(value).toFixed(2);
    },
  },
  methods: {
    ...mapActions(["getProducts"]),
  },
  computed: mapGetters(["allProducts"]),
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
