<script lang="ts">
import productsData from '../assets/products.json'
export default {
  data() {
    return {
      products: productsData,
      selectedProduct: {
        "id": 8,
        "alt": "Green reversing radar",
        "image": "/src/assets/img/products/green_product",
        "icon": "/src/assets/img/products/icons/white_green"
      },
    }
  },
}
</script>

<template>
  <div class="col-md-12 personalization-title">
    <div class="circle">
      <img src="/src/assets/img/anneau_2.svg" alt="anneau">
    </div>
    <div class="title">
      Un large choix de couleurs
    </div>
  </div>
  <div class="col-md-6 personalized-image">
    <img :src="selectedProduct.image" :alt="selectedProduct.alt">
  </div>
  <div class="col-md-6 perzonalization-menu">
    <div class="subtitle">
      Choisissez la couleur qui vous convient le mieux parmi notre large gamme:
    </div>
    <div v-for="product in products"  class="button-product">
      <input type="radio" :value="product" name="product" v-model="selectedProduct" checked>
      <img :src="product.icon" :alt="product.alt">
    </div>
  </div>
</template>