<template>
  <div class="main">
    <form @submit.prevent="onSumbit">
      <input type="text" v-model="title" placeholder="Add product" />
      <input type="text" v-model="price" placeholder="Add price" />
      <input type="submit" value="submit" />
    </form>
  </div>
</template>

<script>
export default {
  name: "AddProduct",
  data() {
    return {
      title: "",
      price: "",
    };
  },
  methods: { onSubmit() {} },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
