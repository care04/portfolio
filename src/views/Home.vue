<template>
  <h2>Shop</h2>
  <div class="shopSection">
    <ShopSectionCard v-for="shop in shops" :key="shop.key" :shop="shop" />
  </div>
</template>
<script lang="ts">
import ShopSectionCard from "@/components/shopSectionCard.vue";
import { defineComponent } from "vue";

export default defineComponent({
  name: "Home",
  components: {
    ShopSectionCard,
  },
  data() {
    return {
        "shops": [
      {
        "name": "Music",
        "key": "lm3",
        "shopCategories": [
          {
            "name": "Books",
            "items": [
              {
                "name": "specific product name",
                "image": "../assets/portraite.png",
                "shortDescription": ""
              }
            ]
          },
          {
            "name": "CD Listen",
            "items": [
              {
                "name": "specific product name",
                "image": "../assets/portraite.png",
                "shortDescription": ""
              }
            ]
          },
          {
            "name": "Lessons",
            "items": [
              {
                "name": "specific product name",
                "image": "../assets/portraite.png",
                "shortDescription": ""
              }
            ]
          }
        ]
      },
      {
        "name": "Art",
        "key": "la3",
        "shopCategories": [
          {
            "name": "Wear",
            "books": [
              {
                "name": "specific product name",
                "image": "../assets/portraite.png",
                "shortDescription": ""
              }
            ]
          },
          {
            "name": "piece",
            "books": [
              {
                "name": "specific product name",
                "image": "../assets/portraite.png",
                "shortDescription": ""
              }
            ]
          },
          {
            "name": "other",
            "books": [
              {
                "name": "specific product name",
                "image": "../assets/portraite.png",
                "shortDescription": ""
              }
            ]
          }
        ]
      },
      {
        "name": "Book",
        "key": "lb3",
        "shopCategories": [
          {
            "name": "supplies",
            "books": [
              {
                "name": "specific product name",
                "image": "../assets/portraite.png",
                "shortDescription": ""
              }
            ]
          },
          {
            "name": "finished",
            "books": [
              {
                "name": "specific product name",
                "image": "../assets/portraite.png",
                "shortDescription": ""
              }
            ]
          }
        ]
      }
    ]
    };
  },
});
</script>
<style scoped>
.shopSection {
  display: inline-flex;
  align-items: center;
}
.h2 {
  text-align: center;
}
</style>
