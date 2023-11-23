<template>
  <swiper
    class="max-h-96 h-full"
    :modules="modules"
    :slides-per-view="1"
    :autoplay="{ delay: 100, disableOnInteraction: false }"
  >
    <swiper-slide v-for="(image, i) in images" :key="i">
      <img class="w-full h-full" style="object-fit: cover" :src="image" alt="image" />
    </swiper-slide>
  </swiper>
</template>

<script setup>
import { ref } from 'vue'
import SwiperClass, { Pagination } from 'swiper'
import { Swiper, SwiperSlide } from 'vue-awesome-swiper'

// import swiper module styles
import 'swiper/css'
import 'swiper/css/pagination'
// more module style...

const modules = ref([Pagination])
const images = ref([
  'https://cdn.britannica.com/49/94449-050-ECB0E7C2/Angkor-Wat-temple-complex-Camb.jpg',
  'https://cdn.britannica.com/49/94449-050-ECB0E7C2/Angkor-Wat-temple-complex-Camb.jpg'
])
</script>
