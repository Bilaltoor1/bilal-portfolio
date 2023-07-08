<template>
  <div class="about-me" id="about-me">
    <div class="section-heading-wrapper">
      <h1 class="about-heading heading-section">About Me </h1>
    </div>
    <div class="about-content section-padding">
      <div class="about-profile">
        <img src="../assets/images/IMG_20230704_104713.png" alt="profile">
      </div>

      <div class="about-description">
        <hr class="hr">
        Hey My Name is Muhammad Bilal Toor i am software engineer . I can work with html css javaScript
        node js nuxt js vue js firebase supabase Mongodb mysql i will prove to be perfect choice for you i have courage
        to work
        with my full efforts and i also try to satisfied my client and always try to be friendly with my client and
        give always my 100% to work ....
      </div>
    </div>
    <!--    <div class="about-img">-->
    <!--      <img src="@/assets/svgs/about.svg" alt="wave">-->
    <!--    </div>-->
  </div>
</template>
<script setup lang="ts">
</script>
<style>
.about-me {
  flex-direction: column;
  align-items: center;
  justify-content: center;
  background-color: var(--text-color);
}

.about-img {
  width: 100%;
  height: 150px;
}

.about-img img {
  top: 0;
  left: 0;
  position: absolute;
  opacity: .5;
}

.about-content {
  width: 100%;
  display: flex;
  justify-content: center;
//margin-top: 1.5rem;
}

.about-profile {
  width: 250px;
  height: 250px;
  border-radius: 100px;
}

.about-profile img {
  object-fit: cover;
  height: 100%;
  border-radius: 300px;
  width: 100%;
}

.about-description {
  width: 60%;
  align-self: center;
  display: flex;
  color: var(--clr-slate600);
}

hr {
  margin: 0 1rem 0 2rem;
}

.about-heading {
//padding-top: 2rem; color: var(--clr-slate600);
}

@media (max-width: 680px) {
  .about-content {
    flex-direction: column;
    align-items: center;
  }

  .about-description {
    display: flex;
    flex-direction: column;
    text-align: justify;
    width: 45ch;
    font-size: .8rem;
  }
  .about-description hr {
    margin: 1rem 0;
  }
}
</style>
