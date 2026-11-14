<script setup lang="ts">
  import AppSidebar from './components/AppSidebar.vue'
</script>

<template>
  <div class="flex min-h-screen">
    <AppSidebar
 />

    <div class="flex min-w-0 flex-1 flex-col">
      <RouterView />
    </div>
  </div>
</template>

<style scoped></style>
