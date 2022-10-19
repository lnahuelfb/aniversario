<script setup lang="ts">
import HelloWorld from './components/HelloWorld.vue'
import Footer from './components/Footer.vue'
import Header from './components/Header.vue';
</script>

<template>
  <Header />
  <main>
    <HelloWorld />
  </main>
  <Footer />
</template>

<style scoped>
main {
  margin: 50px 0;
  box-sizing: border-box;
  /* overflow: hidden; */
}
</style>
