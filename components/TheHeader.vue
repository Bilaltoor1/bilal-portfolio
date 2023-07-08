<template>
  <div class="header">
    <h3 class="logo">Bilal Toor</h3>
    <ul class="header-list">
      <li class="header-list-item">
        <a href="#about-me">About</a>
      </li>
      <li class="header-list-item">
        <a href="#projects">Projects</a>
      </li>
      <li class="header-list-item">
        <a href="#skills">Skills</a>
      </li>
    </ul>
    <button class="header-button">
      Contact Me
      <Icon name="mdi:arrow-right-thin" size="1.5em"/>
    </button>
    <div class="mobile-nav" @click="showMobileNav">
      <Icon name="ri:menu-fill" size="1.8em"/>
    </div>
    <div class="mobile-nav-container" v-show="isShow">
      <ul class="mobile-header-list">
        <li class="mobile-header-list-item">
          <a href="#about-me" @click="isShow = false">About</a>
        </li>
        <li class="mobile-header-list-item">
          <a href="#projects" @click="isShow = false">Projects</a>
        </li>
        <li class="mobile-header-list-item">
          <a href="#skills" @click="isShow = false">Skills</a>
        </li>
      </ul>
      <button class="mobile-header-button">
        Contact Me
        <Icon name="mdi:arrow-right-thin" size="1.5em" color="white"/>
      </button>
      <button class="close-mobile" @click="showMobileNav">
        &cross;
      </button>
    </div>
  </div>
</template>

<style scoped>
.header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 45px;
  margin-top: 1rem;
  padding-left: 1rem;
  padding-right: 1rem;
}

.header-list {
  display: flex;
}

.header-list-item:not(:first-of-type) {
  margin-left: 1.4rem;
}

.header-list-item a {
  font-size: 1rem;
  font-weight: 600;
  color: var(--text-color);
}

.header-button {
  background-color: var(--text-color);
  color: var(--clr-slate800);
  display: flex;
  width: 170px;
  height: 100%;
//padding: 18px 42px; justify-content: center; align-items: center; gap: 10px; border-radius: 5px; font-size: 1rem;
}

.logo {
  font-size: 2rem;
  font-family: 'Cookie', cursive;
  color: var(--text-color);
}

.mobile-nav {
  display: none;
}

.open {
  display: flex;
}

.mobile-header-list {
  display: flex;
  flex-direction: column;
}

.mobile-header-list-item {
  margin-bottom: 2.5rem;
}

.mobile-header-list a {
  font-size: 2rem;
  color: var(--text-color);
}

.mobile-header-button {
  border: 1px solid var(--text-color);
  width: 170px;
  height: 45px;
}

.close-mobile {
  position: absolute;
  top: 2rem;
  right: 2rem;
  font-size: 2rem;
}

@media (max-width: 1024px) {
  .mobile-nav {
    display: block;
  }

  .mobile-nav-container {
    display: flex;
    background-color: var(--clr-slate800);
    min-width: 100vw;
    min-height: 100vh;
    overflow: hidden;
    z-index: 200;
    flex-direction: column;
    position: fixed;
    top: 0;
    left: 0;
    color: var(--text-color);
    justify-content: center;
    align-items: center;
    transition: all .5s;
  }

  .header-list {
    display: none;
  }

  .header-button {
    display: none;
  }

  body {
    overflow: hidden;
  }

}
</style>
<script setup>
const isShow = ref('false');
const showMobileNav = () => {
  isShow.value = !isShow.value
}
</script>