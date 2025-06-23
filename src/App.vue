<template>
  <Navbar></Navbar>
  <HomeView></HomeView>
</template>

<script>
import Navbar from './components/Navbar.vue'
import HomeView from './views/HomeView.vue'

export default {
  name: 'App',
  components: {
    Navbar,
    HomeView,
  },
}
</script>

<style>
@import './assets/main.css';
</style>
