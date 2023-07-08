<template>
  <section class="section-padding" id="contact">
    <h1 class="contact-heading heading-section">Contact form</h1>

    <div class="form-container">
      <form
          action="https://formspree.io/f/meqbqgey"
          method="POST"
      >
        <label class="label">
          Your email:
          <input type="email" name="email">
        </label>
        <label class="label">
          Your message:
          <textarea name="message" ></textarea>
        </label>
        <!-- your other form fields go here -->
        <button type="submit" class="contact-button">Send</button>
      </form>
    </div>
  </section>
</template>

<style>
section {
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

.form-container {
  display: flex;
  flex-direction: column;
  max-width: 400px;
  margin: 0 auto;
  padding: 20px;
  background-color: var(--clr-light);
}

.form-container label {
  color: var(--clr-slate800);
  display: block;
  margin-bottom: 1rem;
  text-align: center;
}

.form-container input,
.form-container textarea {
  padding: 8px;
  border: 1px solid var(--clr-slate800);
  width: 100%;
}

.form-container button {
  padding: 10px;
  background-color: var(--clr-slate800);
  color: white;
  border: none;
  cursor: pointer;
  width: 100%;
  text-align: center;
}
.label{
  display: flex;
  align-items: center;
  justify-content: center;
}
@media (max-width: 800px) {
  .contact-heading{
    font-size: 1.4rem;
  }
}
</style>
<script setup lang="ts">
</script>