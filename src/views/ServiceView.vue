<script setup lang="ts">
import TheWelcome from '../components/TheWelcome.vue'
</script>

<template>
  <main>
    <div>
      <TheWelcome />
    </div>
  </main>
</template>


<style>
@media (min-width: 1024px) {
  .service {
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