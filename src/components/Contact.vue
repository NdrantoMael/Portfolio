<template>
    <footer class="w-full py-6 text-center text-gray-300">
      <h2 class="text-4xl font-bold text-center mb-12 text-green-400">Contacts</h2>
      <div class="flex justify-center space-x-6">
        <a
          v-for="link in socialLinks"
          :key="link.name"
          :href="link.url"
          target="_blank"
          class="w-20 h-20 flex items-center justify-center bg-gray-700 rounded-full transition hover:bg-gray-600"
        >
          <img :src="link.icon" :alt="link.name" class="w-10 h-10" />
        </a>
      </div>
    </footer>
  </template>
  
  <script setup>
  const socialLinks = [
    { name: 'GitHub', icon: '/src/images/github.png', url: '#' },
    { name: 'LinkedIn', icon: '/src/images/linkedin.png', url: '#' },
    { name: 'Facebook', icon: '/src/images/facebook.png', url: '#' },
    { name: 'Gmail', icon: '/src/images/gmail.png', url: '#' },
  ];
  </script>
  