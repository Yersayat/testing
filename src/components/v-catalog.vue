<template>
  <div class="v-catalog">
    <h1>Catalog</h1>
    <div class="v-catalog__list">
    <v-catalog-item 
    v-for="product in products"
    :key="product.article"
    v-bind:product_data="product"
    @sendArticle="showChildArticleInConsole"
      
    />

  </div>
  </div>
</template>

<script>

import vCatalogItem from './v-catalog-item.vue'
export default {
  name: 'v-catalog',
  components: {
    vCatalogItem
  },
  props: {},
  data() {
    return {
      products: [
      {
        image: "1.jpg",
        name: "Футболка черная",
        price: 2100,
        article: "T1",
        available: true,
        category: "Мужские"
      },
      {
        image: "2.jpg",
        name: "Кружка чераня",
        price: 3150,
        article: "T2",
        available: true,
        category: "Кружки"
      },
      {
      image: "3.jpg",
      name: "Электрочайник",
      price: 4200,
      article: "jkasjdhashdjahk",
      available: false,
      category: "Кружки"
    },
    {
      image: "4.jpg",
      name: "Нож Кухонный",
      price: 5300,
      article: "T4",
      available: true,
      category: "Кружки"
    },
    {
      image: "5.jpg",
      name: "Утюг",
      price: 6500,
      article: "T5",
      available: false,
      category: "Бытовые"
    }

      ]
    }
  },

  computed: {},
  methods:{
    showChildArticleInConsole(data) {
      console.log(data)
    }
  }
}
</script>

<style lang="scss">
.v-catalog {
&__list{
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  align-items: center;
}
}
</style>
