<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png" />
    <Products> </Products>
    <AddProduct></AddProduct>
  </div>
</template>

<script>
// @ is an alias to /src
import Products from "@/components/Products.vue";
import AddProduct from "../components/AddProduct.vue";

export default {
  name: "Home",
  components: {
    Products,
    AddProduct,
  },
};
</script>
    AddProduct
