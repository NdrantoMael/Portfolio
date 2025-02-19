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
    { name: 'GitHub', icon: '/public/images/github.png', url: 'https://github.com/NdrantoMael' },
    { name: 'LinkedIn', icon: '/public/images/linkedin.png', url: 'https://www.linkedin.com/in/ndranto-mael-6099352a3/' },
    { name: 'Facebook', icon: '/public/images/facebook.png', url: 'https://www.facebook.com/profile.php?id=100041182233823' },
    { name: 'Gmail', icon: '/public/images/gmail.png', url: 'https://mail.google.com/mail/u/0/?pli=1#inbox' },
  ];
  </script>
  