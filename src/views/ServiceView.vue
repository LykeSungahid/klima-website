<script setup lang="ts">
import TheWelcome from '../components/TheWelcome.vue'
</script>

<template>
  <main>
    <div class="service">
      <TheWelcome />
    </div>
  </main>
</template>


<style>
@media (min-width: 1024px) {
  main{
    padding-left: 50px;
  }
  .service {
    align-items: center;
    font-family: 'Courier New', Courier, monospace;
    margin-left: 100px;
    margin-right: 50px;
    font-size: 20px;
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