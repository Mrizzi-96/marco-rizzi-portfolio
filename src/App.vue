<template>
  <Navbar></Navbar>
  <HomeView></HomeView>
  <AboutView></AboutView>
  <SkillsView></SkillsView>
  <PortfolioView></PortfolioView>
  <ContactView></ContactView>
  <Footer></Footer>
</template>

<script>
import Navbar from './components/Navbar.vue'
import AboutView from './views/AboutView.vue'
import ContactView from './views/ContactView.vue'
import HomeView from './views/HomeView.vue'
import PortfolioView from './views/PortfolioView.vue'
import SkillsView from './views/SkillsView.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Navbar,
    HomeView,
    AboutView,
    SkillsView,
    PortfolioView,
    ContactView,
    Footer,
  },
}

document.querySelectorAll('.nav-link').forEach((link) => {
  if (link.href === window.location.href) {
    link.classList.add('active')
    link.setAttribute('aria-current', 'page')
  }
})
</script>

<style>
@import './assets/main.css';
</style>
