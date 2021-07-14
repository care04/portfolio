<template>
  <div class="shop-section-card">
    <h3>{{ shop.name }}</h3>
    <p v-for="category in shop.shopCategories" :key="category.name">{{ category.name }}</p>
  </div>
</template>

<script lang="ts">
export default {
  name: "ShopCategoryCard",
  props: {
    shop: Object,
  },
};
</script>
<style scoped>
p {
  font-size: 20px;
}
h3 {
  margin: 25px 0 0;
  font-size: 35px;
}
.shop-section-card {
  padding: 20px;
  width: 200px;
  height: 300px;
  border: 5px solid #65768a;
  margin-bottom: 18px;
  margin-right: 20px;
  background-color: rgb(188, 199, 188);
  align-content: center;
}
.underLiner {
  size: 40px;
}
.Divider {
  font-size: 30px;
}
</style>
