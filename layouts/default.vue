<template>
  <div>
    <header>
      <!-- Header content -->
      <TheHeader/>
    </header>
    <main class="main-part">
      <slot/> <!-- This will render the page content -->
    </main>
    <footer>
      <!-- Footer content -->
    </footer>
  </div>
</template>
<style>
body{
  background-color: var(--clr-slate600);
  overflow-x:hidden ;
}
</style>
