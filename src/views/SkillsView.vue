<template>
  <section id="skills" class="bg-dark">
    <div class="container">
      <h2 class="section-header">Skills</h2>
      <div class="row row-cols-sm-2 row-cols-lg-3 g-3 pt-3 justify-content-around">
        <div class="col-auto">
          <div class="d-flex flex-column align-items-center justify-content-center">
            <font-awesome-icon :icon="['fas', 'fa-code']" class="icon-custom" />
            <h5 class="skills-header border-bottom w-100">Languages</h5>
            <p>C#, C++, Python, Gdscript, C, Java, Javascript, SQL, Ruby, PHP</p>
          </div>
        </div>
        <div class="col-auto">
          <div class="d-flex flex-column align-items-center justify-content-center">
            <font-awesome-icon :icon="['fas', 'fa-cubes']" class="icon-custom" />
            <h5 class="skills-header border-bottom w-100">Frameworks</h5>
            <p>.NET, Vue.js, jQuery, React, Angular, Bootstrap</p>
          </div>
        </div>
        <div class="col-auto">
          <div class="d-flex flex-column align-items-center justify-content-center">
            <font-awesome-icon :icon="['fas', 'fa-database']" class="icon-custom" />
            <h5 class="skills-header border-bottom w-100">Databases</h5>
            <p>Microsoft SQL Server, MySQL, PostgreSQL</p>
          </div>
        </div>
        <div class="col-auto">
          <div class="d-flex flex-column align-items-center justify-content-center">
            <font-awesome-icon :icon="['fab', 'unity']" class="icon-custom" />
            <h5 class="skills-header border-bottom w-100">Game Engines</h5>
            <p>Unity, Godot, Unreal Engine, Game Maker Studio</p>
          </div>
        </div>
        <div class="col-auto">
          <div class="d-flex flex-column align-items-center justify-content-center">
            <font-awesome-icon :icon="['fas', 'fa-tools']" class="icon-custom" />
            <h5 class="skills-header border-bottom w-100">Operating systems & tools</h5>
            <p>
              MacOS, Ubuntu, Windows, Agile, Taiga, Git, Docker, ElasticSearch, Kibana, LogStash
            </p>
          </div>
        </div>
        <div class="col-auto">
          <div class="d-flex flex-column align-items-center justify-content-center">
            <font-awesome-icon :icon="['fas', 'fa-laptop-code']" class="icon-custom" />
            <h5 class="skills-header border-bottom w-100">Web technologies</h5>
            <p>HTML, CSS, Dashboarding, Github pages, Gitlab</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style>
.icon-custom {
  font-size: 2rem;
  color: var(--portfolio-primary);
  text-align: center;
}
.skills-header {
  color: var(--portfolio-primary);
  text-align: center;
  padding-bottom: 0.5rem;
}
</style>
