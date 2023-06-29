<script setup>
import HelloWorld from './components/HelloWorld.vue'
import Profile from './components/profile.vue'
import Research from './components/Research.vue'
import Works from './components/Works.vue'
import Contact from './components/Contact.vue'
</script>

<template>
  <h1>ポートフォリオ</h1>
  <Profile />
  <Research />
  <Works />
  <Contact />
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
