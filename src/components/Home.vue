<template>
  <div class="flex flex-col md:flex-row items-center justify-between min-h-screen bg-black text-white px-24 gap-20">
    <div class="md:w-1/2 flex justify-center order-last md:order-first">
      <Intro />
    </div>
    <div class="md:w-1/2 flex justify-end md:justify-end lg:pl-64 order-first md:order-last mt-16 sm:mt-20 md:mt-0"> <!-- Ajout de marge en petit écran -->
      <Profile />
    </div>
  </div>
</template>

<script>
import Intro from './Intro.vue';
import Profile from './Profile.vue';

export default {
  components: {
    Intro,
    Profile
  }
};
</script>

<style scoped>
</style>
