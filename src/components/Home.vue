<script setup lang="ts">
import TypingEffect from './TypingEffect.vue';
// Smooth scroll
const scrollToSection = (id: string) => {
    const element = document.getElementById(id);
    if (element) {
        const yOffset = -80; // offset for fixed header
        const y = element.getBoundingClientRect().top + window.pageYOffset + yOffset;
        window.scrollTo({ top: y, behavior: 'smooth' });
    }
};
</script>

<template>
    <!-- Home Section -->
    <main class="pt-18">
        <section id="home"
            class="min-h-[90vh] flex items-center justify-center p-6 bg-gray-100 dark:bg-gray-900 transition-colors duration-200">
            <div class="container mx-auto max-w-7xl flex flex-col md:flex-row items-center justify-between text-center md:text-left gap-12">

                <!-- Text Content -->
                <div class="md:w-1/2 order-2 md:order-1">
                    <h1
                        class="text-4xl md:text-6xl font-extrabold text-gray-900 dark:text-white mb-4 animate-fade-in-down">
                        Julfikar Ali
                    </h1>

                    <!-- Typing Effect H2 -->
                    <h2 class="text-2xl md:text-3xl font-semibold text-teal-600 dark:text-teal-400 mb-6 relative">
                        I'm a <TypingEffect />
                    </h2>

                    <p class="text-lg md:text-xl text-gray-700 dark:text-gray-300 mb-8 max-w-xl mx-auto md:mx-0 animate-fade-in-up">
                        A passionate Full Stack Web Developer with over 4 years of experience, specializing in building
                        high-performance web applications using modern technologies like Laravel and Vue.js.
                    </p>

                    <div class="flex flex-col sm:flex-row items-center space-y-4 sm:space-y-0 sm:space-x-4 mb-8">
                        <button @click="scrollToSection('contact')"
                            class="w-full sm:w-auto bg-teal-600 text-white font-semibold py-3 px-8 rounded-full shadow-lg hover:bg-teal-700 transition-colors duration-200 transform hover:scale-105">
                            Hire Me
                        </button>
                        <a href="/Julfikar Ali_Software_Resume.pdf"
                            class="w-full sm:w-auto text-teal-600 dark:text-teal-400 font-semibold py-3 px-8 rounded-full border border-teal-600 dark:border-teal-400 hover:bg-teal-600 dark:hover:bg-teal-400 hover:text-white transition-colors duration-200">
                            Download CV
                        </a>
                    </div>

                    <!-- Social Links -->
                    <div
                        class="flex justify-center md:justify-start space-x-6 text-gray-500 dark:text-gray-400 text-3xl">
                        <a href="https://github.com/julfikariu" target="_blank"
                            class="hover:text-teal-600 dark:hover:text-teal-400 transition-colors duration-200">
                            <i class="fab fa-github"></i>
                        </a>
                        <a href="https://linkedin.com/in/julfikar-fsdev" target="_blank"
                            class="hover:text-teal-600 dark:hover:text-teal-400 transition-colors duration-200">
                            <i class="fab fa-linkedin"></i>
                        </a>
                    </div>
                </div>

                <!-- Profile Picture -->
                <div class="md:w-1/2 flex justify-center items-center order-1 md:order-2">
                    <div class="relative group">
                        <img src="/1julfikar.jpg" alt="Julfikar Ali"
                            class="rounded-full border-4 border-gray-300 dark:border-gray-700 shadow-2xl w-56 h-56 md:w-80 md:h-80 object-cover transform transition-transform duration-200 group-hover:scale-105">
                        <div
                            class="absolute inset-0 bg-teal-400 dark:bg-teal-500 rounded-full opacity-10 blur-xl transform scale-110 group-hover:scale-125 transition-all duration-200">
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </main>
</template>