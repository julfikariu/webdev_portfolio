<script setup lang="ts">

</script>

<template>
     <!-- Home Section -->
        <section id="home" class="mt-20 min-h-[80vh] flex items-center justify-center p-6">
            <div class="container mx-auto max-w-7xl flex flex-col md:flex-row items-center justify-between text-center md:text-left gap-12">
                <!-- Text Content -->
                <div class="md:w-1/2 order-2 md:order-1">
                    <h1 class="text-4xl md:text-6xl font-extrabold text-white mb-4 animate-fade-in-down">
                        Julfikar Ali
                    </h1>
                    <!-- Typing Effect H2 with a cursor -->
                    <h2 class="text-2xl md:text-3xl font-semibold text-teal-400 mb-6 relative">
                        I'm a <span id="typing-text"></span><span class="font-bold text-gray-400 animate-pulse">|</span>
                    </h2>
                    <p class="text-lg md:text-xl text-gray-400 mb-8 max-w-xl mx-auto md:mx-0 animate-fade-in-up">
                        A passionate Full Stack Web Developer with over 4 years of experience, specializing in building high-performance web applications using modern technologies like Laravel and React.js.
                    </p>
                    <div class="flex flex-col sm:flex-row items-center space-y-4 sm:space-y-0 sm:space-x-4 mb-8">
                        <a href="#contact" class="w-full sm:w-auto bg-teal-500 text-white font-semibold py-3 px-8 rounded-full shadow-lg hover:bg-teal-600 transition-colors duration-300 transform hover:scale-105">
                            Hire Me
                        </a>
                        <a href="#" class="w-full sm:w-auto text-teal-400 font-semibold py-3 px-8 rounded-full border border-teal-400 hover:bg-teal-400 hover:text-white transition-colors duration-300">
                            Download CV
                        </a>
                    </div>
                    <!-- Social Links -->
                    <div class="flex justify-center md:justify-start space-x-6 text-gray-400 text-3xl">
                        <a href="https://github.com/julfikariu" target="_blank" class="hover:text-teal-400 transition-colors duration-300">
                            <i class="fab fa-github"></i>
                        </a>
                        <a href="https://linkedin.com/in/julfikar-fsdev" target="_blank" class="hover:text-teal-400 transition-colors duration-300">
                            <i class="fab fa-linkedin"></i>
                        </a>
                    </div>
                </div>
                <!-- Profile Picture -->
                <div class="md:w-1/2 flex justify-center align-center order-1 md:order-2">
                    <div class="relative group">
                        <img src="/1julfikar.jpg" alt="Julfikar Ali" class="rounded-full border-4 border-gray-700 shadow-2xl w-56 h-56 md:w-80 md:h-80 object-cover transform transition-transform duration-500 group-hover:scale-105">
                        <div class="absolute inset-0 bg-teal-400 rounded-full opacity-20 blur-xl transform scale-110 group-hover:scale-125 transition-all duration-500"></div>
                    </div>
                </div>
            </div>
        </section>
</template>