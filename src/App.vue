<script setup lang="ts">
import Footer from './components/Footer.vue'
import Header from './components/Header.vue'
import Cards from './components/Cards.vue'
</script>

<template>
  <Header />
  <main>
    <Cards />
  </main>
  <Footer />
</template>

<style scoped>
main {
  box-sizing: border-box;
  max-width: 900px;
  margin: 0 auto;
}
</style>
