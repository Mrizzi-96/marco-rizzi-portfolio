<script setup>
import Timeline from 'v-tmline'

const workTimelineItems = [
  {
    id: 1,
    workplace: 'Ramaplast S.p.A.',
    role: 'Software developer',
    period: 'Sept, 2021 – Present, Italy',
    pointsList: [
      'Designing and developing useful software using C# and .NET Core, to speed up and improve the plastic manufacturing production processes.',
      "Maintaining the company's IT infrastructure and website using various JS libraries and frameworks such as JQuery, Bootstrap etc.",
      'Working on a company help desk to solve IT-related problems.',
    ],
  },
  {
    id: 2,
    workplace: 'Indie videogame: Until The Last Plane',
    role: 'Game tester',
    period: 'Sept, 2020 – Jun, 2021, Italy',
    pointsList: ['a', 'b', 'c'],
  },
  {
    id: 3,
    workplace: 'Milan RSE Laboratory',
    role: 'Formative stage',
    period: 'Apr, 2019 – Dec, 2019, Italy',
    pointsList: [
      'Tested CarloC\'s "Until The Last Plane" videogame\'s main gameplay loop, mechanics, economy and balance while pinpointing bugs to contriute to the improvement of the game experience.',
    ],
  },
]
</script>
<template>
  <div class="about bg-custom">
    <div class="container">
      <div class="row align-items-center py-4">
        <div class="col">
          <h1 class="display-5">About me</h1>
        </div>
      </div>
    </div>
  </div>
  <div class="container">
    <div class="row row-cols-2 g-3">
      <div class="col-lg-6">
        <h4 class="border-bottom">Experiences</h4>
        <Timeline :items="workTimelineItems">
          <template #item="{ item }">
            <div class="custom-timeline-content">
              <p class="title">{{ item.workplace }}</p>
              <p class="role">{{ item.role }}</p>
              <p class="period form-text">{{ item.period }}</p>
              <ul>
                <li v-for="bullet in item.pointsList">{{ bullet }}</li>
              </ul>
            </div>
          </template>
        </Timeline>
      </div>
      <div class="col-auto">
        <h4>Education</h4>
      </div>
    </div>
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 5vh;
    display: flex;
    align-items: center;
  }
}
p {
  margin-bottom: 0;
}
.title {
  font-size: 20px;
  font-weight: bold;
  margin-bottom: 0;
}
.role {
  font-size: 16px;
  /* font-weight: lighter; */
}
</style>
