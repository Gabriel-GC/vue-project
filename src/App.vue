<script setup>
import ProductList from './components/ProductList.vue'
// import Splide from './components/Slider.vue';
</script>

<template>
  <section class="container">
    <!-- <Splide ref="splide"/> -->
    <div class="list-content">
      <h1>Minha Loja Online</h1>
      <ProductList :products="products" />
    </div>
  </section>
</template>

<script>
export default {
  name: 'App',
  components: {
    ProductList
  },
  data() {
    return {
      products: [
        { id: 1, name: 'Camiseta', price: 29.99 },
        { id: 2, name: 'Calça Jeans', price: 59.99 },
        { id: 3,  name: 'Tênis', price: 290.99 },
        { id: 4,  name: 'Bermuda', price: 149.99 },
        { id: 5,  name: 'Boné', price: 89.99 },
        { id: 6,  name: 'Luva', price: 29.99 },
        { id: 7,  name: 'Pulseira', price: 129.99 },
        { id: 8,  name: 'Palmilha', price: 19.99 }
      ],
    }
  }
}
</script>
