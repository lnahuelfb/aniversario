<script setup lang="ts">
import { data } from '../data';
import Cards from './Cards.vue'

</script>

<template>

  <div class="container">
    <!-- <Cards v-for="(message, index) in data" :message="message.message" :image="message.image || undefined" :key="index" /> -->
    <Cards/>
  </div>

</template>

<style scoped>

</style>
