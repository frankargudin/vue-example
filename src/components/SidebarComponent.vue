<template>
  <div class="sidebar">
    <h2>Brra Lateral</h2>
    <ul>
      <li><router-link to="/contador">Contador</router-link></li>
      <li><router-link to="/lista-de-tareas">Lista De Tareas</router-link></li>
    </ul>
  </div>
</template>

<script setup lang="ts"></script>

<style lang="css" scoped>
.sidebar {
  width: 200px;
  background-color: purple;
  padding: 20px;
}
</style>
