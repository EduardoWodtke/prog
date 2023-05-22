<script setup>
  import { livros } from "@/_data/livros"
</script>

<template>
  <h1>MINDE</h1>
  <div class="livro">
  <div class="card-livros" v-for="livro in livros" :key="livro.id">
    <img src="livro.cover" alt="" class="livro-capa">
    <p class="livro-titulo">{{ livro.title }}</p>
    <p class="livro-autor">{{ livro.author }}</p>
    <p class="livro-preco">{{ livro.price }}</p>
  </div>
  </div>
</template>

<style scoped>

</style>
