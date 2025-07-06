<template>
  <nav class="navbar navbar-expand-lg fixed-top dark-bg" data-bs-theme="dark">
    <div class="container">
      <a class="navbar-brand" href="#">
        <div class="navbar-logo">
          <img src="/favicon.ico" class="nav-icon" />
        </div>
      </a>
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarNavAltMarkup"
        aria-controls="navbarNavAltMarkup"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"
          ><i class="fas fa-bars" style="color: #fff; font-size: 28px"></i
        ></span>
      </button>
      <div id="navbarNavAltMarkup" class="collapse navbar-collapse">
        <ul id="navbar-nav" class="navbar-nav ms-lg-auto align-items-center">
          <li class="active-nav">
            <a class="nav-item nav-link" href="#">Home</a>
          </li>
          <li><a class="nav-item nav-link" href="#about">About</a></li>
          <li><a class="nav-item nav-link" href="#skills">Skills</a></li>
          <li><a class="nav-item nav-link" href="#portfolio">Portfolio</a></li>
          <li><a class="nav-item nav-link" href="#contact">Contact</a></li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<style>
.header-title__logo {
  font-weight: bold;
  font-size: 1.5rem;
}
ul#navbar-nav > li > a {
  color: var(--nav-text-white);
}

ul#navbar-nav > li > a:hover {
  color: var(--portfolio-primary);
}
#FirstName {
  color: var(--nav-text-white);
}
#LastName {
  color: var(--portfolio-primary);
}
</style>
<script lang="ts">
import data from '../data/data.json'

export default {
  name: 'Header',
  components: {},
  props: {},
  data() {
    return {
      main: data.main,
    }
  },
}
</script>
