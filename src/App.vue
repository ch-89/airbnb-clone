<script setup>
import Navbar from "./components/Navbar.vue"
import Card from "./components/Card.vue"
import { ref } from 'vue';

const cards = ref([
  "london",
  "paris",
  "berlin",
  "rome",
  "madrid",
  "athens",
  "amsterdam",
  "stockholm"
])
</script>

<template>
  <Navbar/>
  <main class="max-w-7xl mx-auto p-8 grid md:grid-cols-4 gap-8">
    <Card v-for="card in cards" :key="card" :card="card" />
  </main>
</template>