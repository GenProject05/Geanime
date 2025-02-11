<script setup lang="ts">
import Navbar from '@/components/Navbar.vue';
import Footer from '@/components/Footer.vue';
import { ref } from 'vue'

const animeList = ref([
  { title: 'Naruto', description: 'A story about a ninja.' },
  { title: 'One Piece', description: 'Pirates searching for the ultimate treasure.' },
  { title: 'Attack on Titan', description: 'Humans fighting against giant creatures.' },
  { title: 'Dragon Ball', description: 'A story about a ninja.' },
  { title: 'My Hero Academia', description: 'A story about a ninja.' },
  { title: 'Demon Slayer', description: 'A story about a ninja.' },
  { title: 'Death Note', description: 'A story about a ninja.' },
  { title: 'Tokyo Ghoul', description: 'A story about a ninja.' },
  { title: 'Black Clover', description: 'A story about a ninja.' },
  { title: 'Bleach', description: 'A story about a ninja.' },
  { title: 'Hunter x Hunter', description: 'A story about a ninja.' },
  { title: 'Sword Art Online', description: 'A story about a ninja.' },
  { title: 'Fairy Tail', description: 'A story about a ninja.' },
  { title: 'One Punch Man', description: 'A story about a ninja.' },
])
</script>

<template>
  <Navbar />
  <main class="bg-gray-100 min-h-screen p-4">
    <h1 class="text-2xl font-bold mb-4">Anime List</h1>
    <ul class="space-y-4">
      <li v-for="anime in animeList" :key="anime.title" class="bg-white p-4 rounded-lg shadow-md">
        <h2 class="text-xl font-semibold">{{ anime.title }}</h2>
        <p class="text-gray-700">{{ anime.description }}</p>
      </li>
    </ul>
  </main>
  <Footer />
</template>

<style scoped>
/* Add any additional styles here */
</style>
