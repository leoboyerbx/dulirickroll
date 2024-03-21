<script setup>
const date = new Date('2024-03-21 11:00:00')
const today = new Date();

let diff = today.getTime() - date.getTime();
const days = Math.round(diff / (1000 * 3600 * 24));
document.title = days + ' days since the last time Duli rickrolled me'

const highScore = 36
</script>

<template>
  <div flex flex-col>
    <h1 text-24 mb-0>{{ days }}</h1>
    <p text-8>days since last time Duli rickrolled me</p>
    <p class="text-4">Highscore: {{ Math.max(highScore, days) }}</p>
  </div>
</template>
