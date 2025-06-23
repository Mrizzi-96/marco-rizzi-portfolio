<template>
  <div class="row arrow-container">
    <a href="#about" class="arrow-icon" role="button">
      <font-awesome-icon :icon="['fas', 'chevron-down']" size="4x" />
    </a>
  </div>
</template>

<script>
import data from '../data/data.json'

export default {
  name: 'Arrow',
  props: {},
  data() {
    return {
      data: data,
    }
  },
}
</script>

<style lang="scss"></style>
