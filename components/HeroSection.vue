<template>
  <div class="hero-section">
    <div class="hero-content section-padding ">
      <h4 class="hero-name">Hey I AM Bilal Toor</h4>
      <h2 class="hero-work">
        As a web developer, I <strong>STRIVE</strong> to create <strong>ENGAGING</strong> and
        <strong>USER-FRIENDLY</strong> digital experiences by combining my passion for design and expertise in coding.

      </h2>
      <p class="hero-description">
        I am an HTML, CSS, JavaScript, Node.js, Vue.js, Nuxt.js,
        MongoDB, Firebase, and Supabase developer. </p>
      <Icon name="mdi:jira" class="content-img" size="4em" color="#475569"/>
    </div>
    <button class="hero-button">
      <a href="#skills">
        SKILLS
        <Icon name="mdi:arrow-right-thin" size="1em"/>
      </a>
    </button>
  </div>
</template>

<style>
.hero-section {
  height: calc(100vh - 60px);
  width: 100%;
  position: relative;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.hero-img {
  width: 100%;
  height: 150px;
}

.hero-img img {
  bottom: 0;
  left: 0;
  position: absolute;
  opacity: .5;
}

.hero-content {
  margin-top: 2rem;
  display: flex;
  flex-direction: column;
  position: relative;
  width: 800px;
  height: 350px;
  background-color: var(--text-color);
  border-radius: 20px;
  padding: 1.5rem;
  box-shadow: 3px 4px 2px 1px rgba(0, 0, 0, 0.2);
}

.content-img {
  position: absolute;
  bottom: 1rem;
  right: 1rem;
//width: 200px; //height: 200px;
}

.hero-name {
  font-family: 'Cookie', cursive;
  font-size: 1.5rem;
  color: var(--clr-slate800);
  margin-bottom: 2rem;
}

.hero-work {
  font-size: 1.4rem;
  text-align: justify;
  word-spacing: 0;
  color: var(--clr-slate800);
}

.hero-work strong {
  color: var(--clr-indigo);
  font-style: italic;
}

.hero-description {
  font-size: 1rem;
  font-weight: 600;
  color: var(--text-color);
}

.hero-button {
  background-color: var(--text-color);
  display: flex;
  width: 170px;
  justify-content: center;
  align-items: center;
  gap: 10px;
  border-radius: 5px;
  font-size: 1rem;
  height: max-content;
  margin-top: 3rem;
  padding: .5rem 2rem;
  font-weight: 500;
}

.hero-button a {
  color: var(--clr-slate800);
}

@media (max-width: 1024px) {
  .hero-content {
    width: 80%;
  }

  .hero-content {
    margin-top: 0;
  }

  .content-img {
    position: absolute;
    bottom: .6rem;
    right: .6rem;
  //width: 200px; //height: 200px;
  }

  .hero-name {
    font-family: 'Cookie', cursive;
    font-size: 1.1rem;
    margin-bottom: 1rem;
  }

  .hero-work {
    font-size: 1.4rem;
  }

  .hero-work strong {
    color: var(--clr-indigo);
    font-style: italic;
  }

  .hero-description {
    font-size: .8rem;
  }

  @media (max-width: 480px) {
    .hero-content {
      width: 96%;
    }

    .hero-section {
      height: 100%;
      margin: 5rem 0;
    }
  }
  @media (max-width: 600px) {
    .hero-work {
      font-size: 1.1rem;
    }


    .hero-work strong {
      font-weight: bold;
      font-style: normal;
    }
  }
}
</style>
<script setup lang="ts">
</script>