<template>
  <h1>Hola Mundo</h1>
  <p>{{ count }}</p>
  <button @click="incrementarCount">Incrementar</button>
  <button @click="decrementarCount">Decrementar</button>
</template>

<script setup lang="ts">
import { ref } from 'vue'

const count = ref(0)

const incrementarCount = () => {
  count.value++
}
const decrementarCount = () => {
  count.value--
}
</script>

<style scoped>
p {
  color: red;
}
</style>
