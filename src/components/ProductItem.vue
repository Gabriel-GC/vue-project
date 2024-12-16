<template>
    <li>
      <img src="https://placehold.co/1000x1500" alt="imagem do produto">
      <p>{{ product.name }} - R$ {{ product.price }}</p>
      <button @click="console.log(`Você adicionou: ${product.name} no carrinho, no valor de: R$${product.price}`)">Adicionar no carrinho</button>
    </li>
  </template>
  
  <script>
  export default {
    name: 'ProductItem',
    props: {
      product: {
        type: Object,
        required: true,
      }
    }
  }
  </script>