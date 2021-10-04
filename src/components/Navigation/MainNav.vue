<template>
  <v-app id="application">
    <div id="nav" aria-label="Main" role="navigation">
      <router-link :to="{ name: 'Home' }">Home</router-link> |
      <router-link :to="{ name: 'About' }">About</router-link>
    </div>

    <main><router-view /></main>
  </v-app>
</template>
<script>
export default {
  name: 'MainNav'
}
</script>
