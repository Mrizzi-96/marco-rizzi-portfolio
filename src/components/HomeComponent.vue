<script setup lang="ts">
import { faItchIo } from '@fortawesome/free-brands-svg-icons'
</script>

<template>
  <div class="container col-xxl-8 px-4 py-5">
    <div class="row flex-lg-row-reverse align-items-center g-5 py-5">
      <div class="col-10 col-sm-8 col-lg-6">
        <img
          src="../assets/profileItch.png"
          class="d-block mx-lg-auto img-fluid img-portrait"
          alt="Bootstrap Themes"
          width="400"
          height="300"
          loading="lazy"
        />
      </div>
      <div class="col-lg-6">
        <h1 class="display-5 fw-bold text-body-emphasis lh-1 mb-3">Hi, I'm Marco Camillo Rizzi.</h1>
        <p class="lead">
          I'm a software developer based in Tortona, Italy, with 3+ years experience in the web
          development world.
          <br />
          Passionate about game developing in any shape or form. I love to play video games in my
          free time and playing the drums in the evening.
        </p>
        <div class="d-grid gap-2 d-md-flex justify-content-md-start">
          <button
            type="button"
            class="btn btn-outline-danger"
            data-bs-toggle="tooltip"
            data-bs-title="Default tooltip"
          >
            <font-awesome-icon :icon="['fab', 'itch-io']" />
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.img-portrait {
  border-radius: 100%;
  border: 1px solid transparent;
}
</style>
