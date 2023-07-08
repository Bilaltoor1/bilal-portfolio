<template>
  <section class="project section-padding" id="projects">
    <div class="section-heading-wrapper">
      <h1 class="project-heading heading-section"> Project </h1>
    </div>
    <div class="project-container">

      <div class="project-item" v-for="project in projects" :key="project.name">
        <div class="img-container">
          <img :src="project.img" alt="img" class="project-img">
        </div>
        <div class="project-content">
          <a href="#" target="_blank" class="github-link">
            <Icon name="tabler:brand-github"/>
          </a>
          <h3 class="project-name">{{ project.name }}</h3>
        </div>
        <button class="read-more">Github link
          <Icon name="mdi:link" size="1em" class="icon"/>
        </button>
      </div>
    </div>
  </section>
</template>
<style>
.project {
  width: 100%;
}

.project-heading {
  text-align: center;
}

.project-container {
  display: flex;
//grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); justify-content: center; margin: 0 auto; flex-wrap: wrap; gap: 3rem;
}

.project-item {
  width: 280px;
  padding-bottom: 1rem;
  border: 1px solid var(--text-color);
  display: flex;
  flex-direction: column;
}

.project-content {
  display: flex;
  justify-content: space-between;
  padding: .5rem;
  align-items: center;
  height: 40%;
}

.project-name {
  order: -1;
  font-size: 1.2rem;
  color: var(--text-color);
  font-family: 'Open Sans', sans-serif;
}

.project-img {
  min-width: 100%;
  min-height: 100%;
  height: 200px;
  object-fit: cover;
}

.img-container {
  width: 100%;
  height: 60%;
}

.github-link {
  color: var(--clr-slate800);
  font-size: 1.5rem;
}

.icon {
  color: var(--clr-slate800);
}

.read-more {
  display: flex;
  width: 150px;
  justify-content: space-around;
  align-items: center;
  gap: 10px;
  border-radius: 5px;
  font-size: 14px;
  background-color: var(--text-color);
  color: var(--clr-slate800);
  height: max-content;
  margin-top: 1rem;
  padding: .5rem 1rem;
  align-self: center;
}
</style>
<script setup>
const projects = ref([
  {
    name: 'Vue js',
    img: '/Cover image.png'
  },
  {
    name: 'nuxt js',
    img: '/Cover image.png'
  },
  {
    name: 'Node js',
    img: '/Cover image.png'
  },
])
</script>