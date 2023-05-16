<script setup lang="ts">
</script>

<template>
  <main>
    <div class="contact">
      <h1>This is Contacts</h1>
    </div>
  </main>
</template>

<style>
@media (min-width: 1024px) {
  .contact {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
  body {
    display: flex;
    place-items: center;
  }

  #app {
    display: grid;
    grid-template-columns: 1fr 1fr;
    padding: 0 2rem;
  }
}
</style>