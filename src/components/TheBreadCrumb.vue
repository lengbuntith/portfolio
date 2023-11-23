<template>
  <div
    class="bg-green-400 w-full h-96 bg-no-repeat bg-center bg-cover bg-[url('https://cdn.britannica.com/49/94449-050-ECB0E7C2/Angkor-Wat-temple-complex-Camb.jpg')]"
  >
    <div class="w-full h-full flex items-center justify-center">
      <h1 class="text-4xl text-white font-bold shadow-sm">{{ title }}</h1>
    </div>
  </div>
</template>

<script setup>
defineProps({
  title: String,
  description: String,
  image: String,
  link: String
})
</script>
