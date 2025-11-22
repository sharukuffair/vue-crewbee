<template>
  <h1 class="text-xl bg-primary-500 text-green-300">You did it!</h1>
  <LoginPage />
  <ProductsGrid />
</template>

<style scoped></style>

<script>
import LoginPage from "@/components/LoginPage.vue";
import ProductsGrid from "@/components/Productgrid.vue";

export default {
  data() {
    return {};
  },
  components: { LoginPage, ProductsGrid },
};
</script>
