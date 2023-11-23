<template>
  <navbar>
    <div class="bg-black w-full h-20 shadow">
      <div class="flex justify-between items-center h-full px-4">
        <div class="flex items-center">
          <router-link to="/" class="text-white text-2xl font-bold">Home</router-link>
        </div>
        <div class="flex items-center">
          <router-link
            to="/projects"
            class="text-black font-medium mr-4 bg-white rounded-xl p-2 shadow-md"
            >Projects</router-link
          >

          <router-link
            to="/experience"
            class="text-black font-medium mr-4 bg-white rounded-xl p-2 shadow-md"
            >Experience</router-link
          >

          <router-link
            to="/education"
            class="text-black font-medium mr-4 bg-white rounded-xl p-2 shadow-md"
            >Education</router-link
          >

          <router-link
            to="/about"
            class="text-black font-medium mr-4 bg-white rounded-xl p-2 shadow-md"
            >About</router-link
          >
        </div>
      </div>
    </div>
  </navbar>
</template>

<script setup></script>

<style lang="scss" scoped></style>
