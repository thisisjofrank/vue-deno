<script setup lang="ts">
import Dinosaurs from './Dinosaurs.vue';
</script>
<template>
  <h1>Welcome to the Dinosaur App! 🦕</h1>
  <p>Click on a dinosaur to learn more about them</p>
  <Suspense>
    <template #default>
      <Dinosaurs />
    </template>
    <template #fallback>
      <div>Loading...</div>
    </template>
  </Suspense>
</template>
