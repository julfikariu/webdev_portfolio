<template>
  <div>
    <!-- Header & Navigation -->
    <header class="fixed w-full top-0 z-50 bg-gray-900 dark:bg-gray-100 bg-opacity-80 backdrop-blur-sm shadow-xl">
      <nav class="container mx-auto max-w-7xl px-6 py-4 flex items-center justify-between">
        <!-- Logo/Name -->
        <a href="#home" class="text-2xl font-bold text-teal-400">Julfikar Ali</a>

        <!-- Desktop Navigation -->
        <ul class="hidden md:flex items-center space-x-6 font-medium text-gray-300 dark:text-gray-700">
          <li><a href="#home" class="hover:text-teal-400 transition-colors duration-300">Home</a></li>
          <li><a href="#about" class="hover:text-teal-400 transition-colors duration-300">About</a></li>
          <li><a href="#experience" class="hover:text-teal-400 transition-colors duration-300">Experience</a></li>
          <li><a href="#skills" class="hover:text-teal-400 transition-colors duration-300">Skills</a></li>
          <li><a href="#projects" class="hover:text-teal-400 transition-colors duration-300">Projects</a></li>
          <li><a href="#education" class="hover:text-teal-400 transition-colors duration-300">Education</a></li>
          <li><a href="#contact" class="hover:text-teal-400 transition-colors duration-300">Contact</a></li>
          
          <!-- Dark Mode Toggle (Desktop) -->
          <li>
            <button @click="toggleTheme" id="theme-toggle-desktop" class="focus:outline-none cursor-pointer">
              <i :class="darkMode ? 'fas fa-moon text-yellow-400' : 'fas fa-sun text-yellow-400'" class="text-xl hover:text-yellow-300 transition-colors duration-300"></i>
            </button>
          </li>
        </ul>

        <!-- Mobile Menu Button -->
        <div class="flex items-center md:hidden space-x-4">
          <button id="theme-toggle-mobile" @click="toggleTheme" class="focus:outline-none cursor-pointer">
            <i :class="darkMode ? 'fas fa-moon text-yellow-400' : 'fas fa-sun text-yellow-400'" class="text-xl hover:text-yellow-300 transition-colors duration-300 cursor-pointer"></i>
          </button>
        </div>
      </nav>
    </header>
  </div>
</template>

<script setup lang="ts">
import { ref, onMounted } from 'vue';

// Ref to hold the theme state
const darkMode = ref(false);

// Toggle the theme
function toggleTheme() {
  darkMode.value = !darkMode.value;
  if (darkMode.value) {
    document.documentElement.classList.add('dark');
    localStorage.setItem('theme', 'dark');
  } else {
    document.documentElement.classList.remove('dark');
    localStorage.setItem('theme', 'light');
  }
}

// Check if a theme is already set in localStorage
onMounted(() => {
  const savedTheme = localStorage.getItem('theme');
  if (savedTheme) {
    darkMode.value = savedTheme === 'dark';
    if (darkMode.value) {
      document.documentElement.classList.add('dark');
    } else {
      document.documentElement.classList.remove('dark');
    }
  }
});
</script>
