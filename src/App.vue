<template>
  <div>
    <NavBar />
    <router-view /> <!-- Si vous utilisez Vue Router -->
  </div>
  <div id="home">
    <Home />
  </div>
  <div id="projects">
    <Projects />
  </div>
  <div id="skills">
    <Skills />
  </div>
  <div id="contact">
    <Contact />
  </div>
</template>

<script setup>
import NavBar from './components/NavBar.vue';
import Home from './components/Home.vue'; // Assurez-vous que le chemin est correct
import Projects from './components/Projects.vue';
import Skills from './components/Skills.vue';
import Contact from './components/Contact.vue';


</script>

<style>
/* Styles globaux si nécessaire */
* {
  font-family: 'Roboto', sans-serif;
  background-color: black;
}
</style>
