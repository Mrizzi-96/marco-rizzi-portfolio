<template>
  <div class="container footer">
    <div class="row justify-content-center align-items-baseline pb-3">
      <div class="col-auto">
        <a :href="footer.linkedinPath" target="_blank">
          <font-awesome-icon class="contact-icon" :icon="['fab', 'linkedin']"
        /></a>
      </div>
      <div class="col-auto">
        <a :href="footer.gitPath" target="_blank"
          ><font-awesome-icon class="contact-icon" :icon="['fab', 'github']"
        /></a>
      </div>
      <div class="col-auto">
        <a :href="footer.itchPath" target="_blank">
          <font-awesome-icon class="contact-icon" :icon="['fab', 'itch-io']"
        /></a>
      </div>
      <div class="col-auto">
        <a :href="footer.instagramPath" target="_blank">
          <font-awesome-icon class="contact-icon" :icon="['fab', 'instagram']"
        /></a>
      </div>
    </div>
    <div class="row justify-content-center">
      <div class="col-12 col-sm-auto text-center">
        <span class="d-block font-monospace copyText">{{ footer.copyrightText }}</span>
      </div>
    </div>
  </div>
</template>

<script lang="js">
import data from '../data/data.json'

export default {
  name: 'Footer',
  components: {},
  props: {},
  data() {
    return {
      footer: data.footer,
    }
  },
}
</script>

<style lang="css">
.footer {
  padding-block: 1rem;
}
.contact-icon {
  font-size: 4rem;
  color: var(--portfolio-primary);
  -moz-transition: all 0.1s ease-in;
  -o-transition: all 0.1s ease-in;
  -webkit-transition: all 0.1s ease-in;
  transition: all 0.1s ease-in;
  cursor: pointer;
}
.contact-icon:hover {
  color: var(--portfolio-secondary);
}
.contact-icon:active {
  color: var(--portfolio-tertiary);
}
.copyText {
  font-size: 0.875rem;
}
</style>
