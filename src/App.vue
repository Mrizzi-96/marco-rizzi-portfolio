<script setup lang="ts">
import ContactView from './views/ContactView.vue'
import Header from './views/Header.vue'
import PortfolioView from './views/PortfolioView.vue'
import SkillsView from './views/SkillsView.vue'
</script>
<template>
  <main>
    <Header></Header>
    <HomeView></HomeView>
    <AboutView></AboutView>
    <SkillsView></SkillsView>
    <PortfolioView></PortfolioView>
    <ContactView></ContactView>
    <Footer></Footer>
  </main>
</template>

<style>
@import './assets/main.css';
</style>
