<template>
  <div class="flex flex-col items-center justify-center min-h-screen bg-black text-white gap-4 mb-8 sm:mb-12 md:mb-0">
    <!-- Texte d'introduction -->
    <p class="text-gray-400 text-lg">Bonjour, je suis</p> 
    <h1 class="text-6xl font-extrabold">
      <span class="text-white">RASEHENONJATOVO </span> 
      <span class="text-green-400">Ndranto Maël.</span>
    </h1>

    <p class="text-gray-400 text-lg text-center max-w-2xl">
      Un développeur et étudiant en informatique passionné par le développement et les nouvelles technologies.
    </p>

    <!-- Bouton de téléchargement du CV -->
    <a 
      href="#" 
      download 
      class="mt-6 px-6 py-3 bg-green-500 text-black font-semibold rounded-lg shadow-md transition duration-300 ease-in-out transform hover:bg-yellow-400 hover:scale-105"
    >
      Télécharger mon CV
    </a>

  </div>
</template>

<style scoped>
.social-btn {
  @apply w-16 h-16 flex items-center justify-center bg-gray-800 rounded-full transition duration-300 hover:bg-gray-600 shadow-lg;
}
.social-btn img {
  @apply w-8 h-8;
}
</style>
