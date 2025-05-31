<script setup lang="ts">
import Navbar from './components/Navbar.vue'
import { RouterView } from 'vue-router'
</script>
<template>
  <main>
    <Navbar></Navbar>
    <RouterView></RouterView>
  </main>
</template>

<style scoped>
main {
  width: 100%;
}
</style>
