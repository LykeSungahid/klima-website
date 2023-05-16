<script setup lang="ts">
defineProps<{
  msg: string
}>()
</script>

<template>
  <div class="greetings">
    <h1 class="green">{{ msg }}</h1>
    <h3>
      Klima Engineering and Services is offering you good quality
    </h3>
    <h3>
      and reliable air-conditioning services.
    </h3>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 5rem;
  top: -10px;
  width: 100%;
  text-align: center;
  font-family: 'Courier New', Courier, monospace;
  font-weight: bold;
}

h3 {
  font-size: 2.5rem;
  width: 100%;
  text-align: center;
  font-family: 'Courier New', Courier, monospace;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: center;
  }
}
</style>
