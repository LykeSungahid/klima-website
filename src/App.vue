<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <header>
    <div class="wrapper">

      <a id="logo" href="/"><img alt="Vue logo" class="logo" src="@/assets/Logo3.svg" width="125" height="125" /></a>

      <HelloWorld id="helloworld" msg="Klima Engineering and Services" />

      <nav>
        <RouterLink to="/about">About</RouterLink>
        <RouterLink to="/services">Services</RouterLink>
        <RouterLink to="/contact">Contact</RouterLink>
      </nav>
    </div>
  </header>
  <RouterView />
</template>

<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
  text-align: center;
  margin-top: 25px;
  margin-bottom: 50px;
}

.logo {
  width: 100%;
  display: block;
  margin: 0 auto 2rem;
}
#logo {
  width: 19%;
  display: block;
  margin: auto;
}

nav {
  width: 100%;
  font-size: 20px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: center;
    flex-wrap: wrap;
    width: 100%;
  }

  nav {
    text-align: center;
    font-size: 20px;
    font-family: 'Courier New', Courier, monospace;
    padding: 1rem 0;
    margin-top: 1rem;
  }
  #helloworld {
    width: 100%;
  }
}

@media (hover: hover) {
  #logo {
    background-color: hsla(0, 0%, 100%, 0.2);
  }
}
</style>
