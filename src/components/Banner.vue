<template>
  <div class="banner">
    <div class="banner-text">
      <h1 class="font-monospace banner-main__title">{{ name.first }} {{ name.last }}</h1>
      <h2 id="typewriter" class="font-monospace"></h2>
    </div>
  </div>
</template>

<script>
import data from '../data/data.json'
import Typewriter from 'typewriter-effect/dist/core'

var titles = data.main.titles

export default {
  name: 'Banner',
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

<style lang="scss"></style>
