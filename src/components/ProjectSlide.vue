<template>
  <div>
    <div class="mb-4">
      <h1 class="text-lg font-bold">My Projects</h1>
      <p class="text-gray-500 font-thin">Latest projects I've been working on.</p>
    </div>

    <swiper
      class="swiper"
      :modules="modules"
      :slides-per-view="1"
      :space-between="10"
      :breakpoints="{
        '640': {
          slidesPerView: 2,
          spaceBetween: 20
        },
        '768': {
          slidesPerView: 4,
          spaceBetween: 40
        },
        '1024': {
          slidesPerView: 5,
          spaceBetween: 50
        }
      }"
    >
      <swiper-slide
        v-for="(project, i) in projects"
        :key="i"
        class="slide shadow rounded overflow-hidden max-h-60"
      >
        <img class="aspect-square" style="object-fit: contain" :src="project" alt="image" />
      </swiper-slide>
    </swiper>
  </div>
</template>

<script setup>
import { ref } from 'vue'
import SwiperClass from 'swiper'
import { Swiper, SwiperSlide } from 'vue-awesome-swiper'

import 'swiper/css'
import 'swiper/css/pagination'

const modules = ref([])

const projects = ref([
  './img/project-1.png',
  './img/project-2.png',
  './img/project-3.png',
  './img/project-4.png'
])
</script>
