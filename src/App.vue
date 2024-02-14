<script setup>
const date = new Date('2024-02-14')
const today = Date.now()

let diff = today.getTime() - date.getTime();
const days = Math.round(diff / (1000 * 3600 * 24));
</script>

<template>
  <div flex flex-col>
    <h1 text-24 mb-0>{{ days }}</h1>
    <p text-8>days since last time Duli rickrolled me</p>
  </div>
</template>
