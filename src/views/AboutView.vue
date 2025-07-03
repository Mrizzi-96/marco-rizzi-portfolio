<template>
  <section id="about">
    <div class="container">
      <h2 class="section-header">About me</h2>
    </div>
    <div class="container">
      <div class="row pt-3">
        <div class="col col-sm-6 col-lg-8">
          <span class="bio">{{ about.bio }}</span>
          <div class="row pt-3">
            <div class="col-12">
              <ul class="list-group list-group-flush facts-list">
                <li class="list-group-item" v-for="fact in about.facts">
                  <h5 class="fact-heading">{{ fact.name }}</h5>
                  <span v-html="fact.value"></span>
                </li>
              </ul>
            </div>
          </div>
        </div>
        <div class="col col-sm-6 col-lg-4">
          <div class="d-flex flex-column align-items-center justify-content-center">
            <img
              class="profile-pic d-block"
              src="../assets/images/profile.jpg"
              alt="profile picture"
            />
            <a
              type="button"
              target="_blank"
              href="CV_RIZZI.pdf"
              download
              class="btn btn-primary resume-btn mt-3"
            >
              <font-awesome-icon :icon="['fas', 'file-arrow-down']" /> Get my resume
            </a>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import data from '../data/data.json'

export default {
  name: 'AboutView',
  components: {},
  props: {},
  data() {
    return {
      about: data.about,
      name: data.main.name.first,
      facts: data.about.facts,
      heading: data.main.headings.about,
    }
  },
}
</script>

<style>
.profile-pic {
  border: 1px solid var(--portfolio-primary);
  aspect-ratio: 4/3;
  width: 15rem;
  height: 15rem;
  object-fit: cover;
  border-radius: 100%;
}
.facts-list {
  background-color: transparent;
}
.facts-list > .list-group-item {
  background-color: transparent;
  color: var(--nav-text-white);
}
.fact-heading {
  font-weight: bold;
}
.resume-btn {
  text-align: center;
}
</style>
