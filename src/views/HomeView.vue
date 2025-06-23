<template>
  <div id="hero">
    <div class="container">
      <div class="title">
        <h1 class="hero__title">Marco Camillo Rizzi</h1>
        <h2 class="hero__subtitle" id="typewriter"></h2>
      </div>
    </div>
  </div>
</template>

<style>
#hero {
  position: relative;
}
#hero > .container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  height: 100%;
}
.hero__title {
  font-size: 4rem;
  margin: 0;
  font-weight: bold;
  color: var(--nav-text-white);
}
.hero__subtitle {
  font-size: 1.5rem;
  font-weight: 700;
  color: var(--portfolio-primary);
}
</style>
<script>
import data from '../data/data.json'
import Typewriter from 'typewriter-effect/dist/core'

var titles = data.main.titles

export default {
  name: 'HomeView',
  data() {
    return {
      name: data.main.name,
      titles: data.main.titles,
    }
  },
  mounted: function () {
    new Typewriter('#typewriter', {
      strings: titles,
      autoStart: true,
      loop: true,
      deleteSpeed: 2,
      delay: 40,
    })
  },
}
</script>
