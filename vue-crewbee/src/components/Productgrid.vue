<template>
  <div style="padding: 20px">
    <Grid
      :style="{ height: '400px' }"
      :data-items="products"
      :columns="columns"
    />
  </div>
</template>

<script>
import { Grid } from "@progress/kendo-vue-grid";

export default {
  name: "ProductsGrid",
  components: {
    Grid,
  },
  data() {
    return {
      products: [
        { id: 1, name: "Phone", price: 10000, category: "Electronics" },
        { id: 2, name: "Laptop", price: 60000, category: "Electronics" },
        { id: 3, name: "Headphones", price: 3000, category: "Accessories" },
      ],
      columns: [
        { field: "id", title: "ID", width: "80px" },
        { field: "name", title: "Product Name" },
        { field: "price", title: "Price" },
        { field: "category", title: "Category" },
      ],
    };
  },
};
</script>
