<template>
  <div class="container">
    <h1>{{message}}</h1>
    <img v-if="image" :src="image" alt=""/>
  </div>
</template>

<script setup lang="ts">
defineProps<{ message: string, image?: string }>()
</script>

<style scoped>

img {
  width: 250px;
  height: 250px;
  object-fit: cover;
  border-radius: 5px;
}

.container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

</style>