<template>
  <div>
    <h2>Lista de Tareas</h2>
    <input type="text" v-model="nuevaTarea" @keyup.enter="addTarea" />
    <ul>
      <li v-for="(tarea, index) in listTareas" :key="index">
        {{ tarea }}
        <button @click="borrarTarea(index)">Borrar Tarea</button>
      </li>
    </ul>
  </div>
</template>

<script lang="ts" setup>
import { ref } from 'vue'

const listTareas = ref<string[]>([])
const nuevaTarea = ref<string>('')

const addTarea = () => {
  listTareas.value.push(nuevaTarea.value || '')
  nuevaTarea.value = ''
}

const borrarTarea = (index: number) => {
  listTareas.value.splice(index, 1)
}
</script>

<style lang="css" scoped></style>
