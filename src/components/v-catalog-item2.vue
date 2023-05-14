<template>
  <div class="v-catalog-item">
<p class="v-catalog-item__name">Name</p>
<img class="v-catalog-item__image" src="" alt="">
<p class="v-catalog-item__price">Price</p>
<button class="v-catalog-item_add_to_cart_btn">Добавить в корзину

</button>

  </div>
</template>

<script>
export default {
  name: 'v-catalog-item2',
  components: {},
  props: {},
  data() {
    return {}
  },
  mounted() {},
  methods: {}
}
</script>

<style lang="scss">
.v-catalog-item2 {
  flex-basis: 25%;
  box-shadow: 0 0 8px 0;
  padding: 16px;
  margin-bottom: 16px;
}
</style>
