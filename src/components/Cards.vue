<template>
  <div class="slider-container">
    <div class="container slider-item" v-for="(card, index) in data" :key="index">
      <h3>{{ card.title }}</h3>
      <span>{{ card.message }}</span>
      <img :src="card.image">
    </div>
  </div>
</template>

<script lang="ts">
import { data } from '../data'

export default {
  name: 'Cards',
  data() {
    return {
      data
    }
  }
}

</script>

<style scoped>
.slider-container {
  box-sizing: border-box;
  width: 100%;
  height: 500px;
  display: flex;
  overflow-x: scroll;
  scroll-snap-type: x proximity;
  overflow-y: hidden;
}

.slider-container div {
  flex: 0 0 100%;
  width: 100%;
  scroll-snap-align: center;
}

.container {
  box-sizing: border-box;
  border-radius: 10px;
  height: max-content;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.container h3 {
  margin: 10px 0 20px 0;
}

.container span {
  margin-bottom: 20px;
}

.container img {
  max-height: 340px;
  max-width: 320px;
  object-fit: cover;
  object-position: center;
}
</style>