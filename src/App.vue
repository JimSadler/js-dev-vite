<script>
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <!-- <div id="flashMessage" v-if="GStore.flashMessage">
    {{ GStore.flashMessage }}
  </div> -->
  <div id="nav" aria-label="Main" role="navigation">
    <div class="main-navigation">
      <div class="logo-container">
        <img src="src/assets/nav-logo.png" alt="" />
      </div>
      <div class="main-nav-links">
        <router-link :to="{ name: 'Home' }">Home</router-link> |
        <router-link :to="{ name: 'About' }">About</router-link> |
      </div>
    </div>
  </div>

  <main><router-view /></main>

  <HelloWorld msg="Hello Vue 3 + Vite" />
</template>

<style>
body {
  margin: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
#nav {
  background-color: lightblue;
}
.logo-container {
  text-align: left;
}
.main-navigation {
  display: flex;
  justify-content: space-between;
  padding: 0.5rem 0.5rem 0 0.5rem;
}
.main-nav-links {
  margin-top: 2.6rem;
  float: right;
}
</style>
