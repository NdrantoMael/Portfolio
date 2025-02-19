<template>
  <nav class="fixed top-0 left-0 w-full bg-black shadow-md z-50">
    <div class="flex justify-center p-4">
      <div class="flex space-x-8 bg-neutral-900 text-gray-400 rounded-full px-6 py-2 shadow-lg">
        <button 
          v-for="(item, index) in menuItems" 
          :key="index"
          @click="scrollToSection(index)"
          class="px-6 py-2 rounded-full transition duration-300 outline-none focus:ring-0 focus:outline-none"
          :class="activeIndex === index ? 'bg-white/20 text-white font-semibold' : 'hover:bg-white/20 hover:text-white'"
        >
          {{ item }}
        </button>
      </div>
    </div>
  </nav>
</template>

<script setup>
import { ref } from 'vue';

const menuItems = ["À propos de moi", "Mes projets", "Mes compétences techniques", "Contact"];
const activeIndex = ref(0);

const scrollToSection = (index) => {
  activeIndex.value = index;
  const sectionId = ["home", "projects", "skills", "contact"][index]; // IDs des sections
  const section = document.getElementById(sectionId);
  if (section) {
    section.scrollIntoView({ behavior: "smooth" });
  }
};
</script>
