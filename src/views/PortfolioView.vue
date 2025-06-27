<template>
  <section id="portfolio">
    <div class="container">
      <h2 class="section-header">My portfolio</h2>
      <div
        :class="
          'pt-3 row row-cols-sm-1 row-cols-md-2 gy-4 align-items-center justify-content-start ' +
          colNumber
        "
      >
        <div class="col-12 col-md-auto" v-for="project in portfolio.projects">
          <div class="portfolio-card">
            <div class="portfolio-details">
              <h3 class="details-title">{{ project.title }}</h3>
              <span>{{ project.description }}</span>
              <a class="btn btn-secondary" target="_blank" :href="project.link">
                <font-awesome-icon :icon="['fas', 'arrow-up-right-from-square']" />
                Website</a
              >
            </div>
            <img class="portfolio-img" :src="project.image" />
            <p class="portfolio-badge-date">Jan 2025</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import data from '../data/data.json'

export default {
  name: 'PortfolioView',
  components: {},
  props: {},
  data() {
    return {
      portfolio: data.portfolio,
      colNumber: data.portfolio.length % 2 == 0 ? 'row-cols-lg-4' : 'row-cols-lg-3',
    }
  },
}
</script>

<style>
.portfolio-card {
  position: relative;
}
.portfolio-card > img {
  object-fit: contain;
  width: 100%;
  height: auto;
  border-radius: 0.35rem;
  aspect-ratio: 16/9;
  border: 0.25rem solid var(--portfolio-secondary);
  box-sizing: border-box;
  object-fit: cover;
}
.portfolio-details {
  position: absolute;
  bottom: 0.2rem;
  left: 0;
  width: 100%;
  height: calc(100% - 0.2rem);
  box-sizing: border-box;
  background-color: var(--portfolio-secondary);
  color: var(--nav-text-white);
  border-radius: 0.35rem;
  text-align: center;
  max-height: 0;
  overflow: hidden;
  padding: 0 1rem;
  transition: 0.15s ease;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 1rem;
}
.portfolio-card:hover > .portfolio-details {
  max-height: 100vh;
  padding: 1rem 1rem 1.5rem;
}

.details-title {
  font-weight: bold;
  width: 100%;
}

.portfolio-badge-date {
  position: absolute;
  bottom: 0.3rem;
  left: 50%;
  transform: translate(-50%, 50%);
  margin: 0;
  border-radius: 100vh;
  background-color: var(--portfolio-secondary);
  color: var(--nav-text-white);
  padding: 0.5em 1em;
  font-weight: 600;
  text-align: center;
}

/* BOOTSTRAP BREAKPOINTS */
/* Small devices (landscape phones, 576px and up) */
@media (min-width: 576px) {
  .portfolio-badge-date {
    font-size: 0.875rem;
  }
}

/* Medium devices (tablets, 768px and up) */
@media (min-width: 768px) {
}

/* Large devices (desktops, 992px and up) */
@media (min-width: 992px) {
}

/* X-Large devices (large desktops, 1200px and up) */
@media (min-width: 1200px) {
}

/* XX-Large devices (larger desktops, 1400px and up) */
@media (min-width: 1400px) {
}
</style>
