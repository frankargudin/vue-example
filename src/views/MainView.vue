<template>
  <div class="container">
    <SidebarComponent></SidebarComponent>
    <div class="content">
      <router-view></router-view>
    </div>
  </div>
</template>

<script setup lang="ts">
import SidebarComponent from '@/components/SidebarComponent.vue'
</script>

<style lang="css" scoped>
.container {
  display: flex;
}

.content {
  flex: 1;
  padding: 20px;
}
</style>
