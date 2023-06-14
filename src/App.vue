<script setup lang="ts">
import HeaderComponent from './components/HeaderComponent.vue'
import SeparatorComponent from './components/SeparatorComponent.vue'
import ProductComponent from './components/ProductComponent.vue'
import SpecsComponent from './components/SpecsComponent.vue'
import VideoComponent from './components/VideoComponent.vue'
import PersonalizationComponent from './components/PersonalizationComponent.vue'

</script>

<template>
  <header>
    <div class="container-fluid header">
      <div class="row">
        <HeaderComponent />
      </div>
    </div>
    <div class="container-fluid separator-container">
      <SeparatorComponent />
    </div>
  </header>

  <main>
    <div class="container-fluid product-container" id="product">
      <ProductComponent />
    </div>
    <div class="container">
      <div class="row">
        <SpecsComponent />
      </div>
    </div>
    <div class="container-fluid">
      <div class="row">
        <VideoComponent />
      </div>
    </div>
    <div class="container-fluid">
      <div class="row">
        <PersonalizationComponent />
      </div>
    </div>
  </main>
</template>
