<template>
  <Navbar></Navbar>
  <HomeView></HomeView>
  <AboutView></AboutView>
  <SkillsView></SkillsView>
  <PortfolioView></PortfolioView>
</template>

<script>
import Navbar from './components/Navbar.vue'
import AboutView from './views/AboutView.vue'
import HomeView from './views/HomeView.vue'
import PortfolioView from './views/PortfolioView.vue'
import SkillsView from './views/SkillsView.vue'

export default {
  name: 'App',
  components: {
    Navbar,
    HomeView,
    AboutView,
    SkillsView,
    PortfolioView,
  },
}
</script>

<style>
@import './assets/main.css';
</style>
