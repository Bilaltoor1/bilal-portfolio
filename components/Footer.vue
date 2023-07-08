<template>
  <section class="container">
    <footer class="footer">
      <div class="footer-bars-container">
        <ul class="footer-list">
          <li class="footer-list-item">
            <NuxtLink to="/">About</NuxtLink>
          </li>
          <li class="footer-list-item">
            <NuxtLink to="/">Projects</NuxtLink>
          </li>
          <li class="footer-list-item">
            <NuxtLink to="/">Skills</NuxtLink>
          </li>
        </ul>
        <ul class="social-media">
          <li>
            <Icon class="icon" name="logos:facebook"></Icon>
          </li>
          <li>
            <Icon class="icon" name="logos:twitter"></Icon>
          </li>
          <li>
            <Icon class="icon" name="logos:instagram-icon"></Icon>
          </li>
          <li>
            <Icon class="icon" name="logos:linkedin-icon"></Icon>
          </li>
          <li>
            <Icon class="icon" name="logos:upwork" size="2em"></Icon>
          </li>
        </ul>
      </div>
      <div class="copyright-text">
        <h3>ALL &copy; Is Reserved By Bilal Toor </h3>
      </div>
    </footer>
  </section>
</template>

<style>
.container {
  background-color: var(--text-color);
}

.footer {
  display: flex;
  flex-direction: column;
  width: 900px;
  margin: 0 auto;
}

.footer-bars-container {
  display: flex;
  justify-content: space-between;
  padding: 2rem 2rem .5rem 2rem;
  align-items: center;
}

.footer-list {
  display: flex;
}

.footer-list-item {
  margin-left: 1rem;
}

.footer-list-item a {
  color: var(--clr-slate800);
}

.social-media {
  display: flex;
  align-items: center;
}

.icon {
  font-size: 1.5rem;
  margin-left: 1rem;
}

.copyright-text {
  text-align: center;
}

.copyright-text h3 {
  color: var(--clr-slate800);
}

@media (max-width: 980px) {
  .footer-bars-container {
    flex-direction: column;
  }

  .footer {
    width: 100%;
  }
  .copyright-text{
    font-size: .9rem;
  }
}
</style>
<script setup lang="ts">
</script>