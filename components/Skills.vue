<template>
  <section class="skills section-padding" id="skills">
    <div class="section-heading-wrapper">
      <h1 class="skills-heading heading-section">
        Skills
      </h1>
    </div>
    <ul class="skills-container">
      <li class="skill-item">
        <Icon name="vscode-icons:file-type-css"  size="2.5em" class="Icon"/>
        <h3>CSS</h3>
      </li>
      <li class="skill-item">
        <Icon name="vscode-icons:file-type-html"   size="2.5em" class="Icon"/>
        <h3>HTML</h3>
      </li>
      <li class="skill-item">
        <Icon name="vscode-icons:file-type-js-official"  size="2.5em" class="Icon"/>
        <h3>JavaScript</h3>
      </li>
      <li class="skill-item">
        <Icon name="vscode-icons:file-type-nuxt"  size="2.5em" class="Icon"/>
        <h3>Nuxt JS</h3>
      </li>
      <li class="skill-item">
        <Icon name="vscode-icons:file-type-vue"  size="2.5em" class="Icon"/>
        <h3>Vue JS</h3>
      </li>
      <li class="skill-item">
        <Icon name="vscode-icons:file-type-light-quasar"  size="2.5em" class="Icon"/>
        <h3>Quasar 2</h3>
      </li>
      <li class="skill-item">
        <Icon name="vscode-icons:file-type-mongo"  size="2.5em" class="Icon"/>
        <h3>MongoDB</h3>
      </li>
      <li class="skill-item">
        <Icon name="vscode-icons:file-type-node"  size="2.5em" class="Icon"/>
        <h3>Node JS</h3>
      </li>
    </ul>
  </section>
</template>

<style>

.skills-container {
  max-width: 900px;
  height: 100%;
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  margin: 2.5rem auto;
  row-gap: 2rem;
}

.skills-heading {
  text-align: center;
}

.skill-item {
  display: flex;
  flex-direction: column;
  align-items: center;
}
.skill-item h3{
  color: var(--text-color);
}

@media (max-width: 580px) {
  .skills-container {
    grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
  }
}


</style>
<script setup lang="ts">
</script>