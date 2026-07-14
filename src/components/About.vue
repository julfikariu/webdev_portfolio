<script setup lang="ts">
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

<section id="about" class="py-16 md:py-20 bg-gray-50 dark:bg-gray-900 transition-colors duration-300">
    <div class="container mx-auto max-w-7xl px-4 sm:px-6 lg:px-8">
        <div class="bg-white dark:bg-gray-800 p-6 md:p-12 lg:p-16 rounded-2xl md:rounded-3xl shadow-lg md:shadow-2xl transition-colors duration-300">
            <!-- Section Header -->
            <div class="text-center mb-12">
                <h2 class="text-2xl sm:text-3xl md:text-4xl font-extrabold text-teal-600 dark:text-teal-400 mb-4">
                    About Me
                </h2>
        
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-3 gap-8 md:gap-12 lg:gap-16 items-start">
                

                <!-- Content Section -->
                <div class="lg:col-span-3 space-y-6 md:space-y-8">
                    <!-- Introduction -->
                    <div>
                        <h4 class="text-xl md:text-2xl font-bold text-gray-900 dark:text-white mb-4">
                            Hello, I'm Julfikar Ali
                        </h4>

                        <p class="text-gray-600 dark:text-gray-300 leading-relaxed md:leading-loose text-sm md:text-base">
                            I am a  Full-Stack Engineer and Systems Architect with over 5 years of experience specializing in high-performance Laravel ecosystems and robust Vue 3 applications. My core expertise lies in designing scalable architectures, automating complex pipelines, developing third-party API sync engines, and optimizing databases for massive data aggregations. I thrive on solving complex engineering challenges and delivering secure, production-ready enterprise solutions that drive measurable business impact.
                        </p>
                    </div>

                    <!-- Quick Highlights Grid -->
                    <div class="grid grid-cols-1 sm:grid-cols-2 gap-4 md:gap-6">
                        <div class="bg-gray-50 dark:bg-gray-700/50 p-4 rounded-xl border border-gray-100 dark:border-gray-600">
                            <p class="font-semibold text-gray-800 dark:text-gray-100 text-sm md:text-base">Experience</p>
                            <p class="text-gray-500 dark:text-gray-300 text-sm mt-1">5+ years building web apps</p>
                        </div>
                        <div class="bg-gray-50 dark:bg-gray-700/50 p-4 rounded-xl border border-gray-100 dark:border-gray-600">
                            <p class="font-semibold text-gray-800 dark:text-gray-100 text-sm md:text-base">Location</p>
                            <p class="text-gray-500 dark:text-gray-300 text-sm mt-1">Dhaka, Bangladesh</p>
                        </div>
                        <div class="bg-gray-50 dark:bg-gray-700/50 p-4 rounded-xl border border-gray-100 dark:border-gray-600">
                            <p class="font-semibold text-gray-800 dark:text-gray-100 text-sm md:text-base">Primary Stack</p>
                            <p class="text-gray-500 dark:text-gray-300 text-sm mt-1">Laravel • Vue.js • MySQL</p>
                        </div>
                        <div class="bg-gray-50 dark:bg-gray-700/50 p-4 rounded-xl border border-gray-100 dark:border-gray-600">
                            <p class="font-semibold text-gray-800 dark:text-gray-100 text-sm md:text-base">Availability</p>
                            <p class="text-gray-500 dark:text-gray-300 text-sm mt-1">Open to freelance & full-time</p>
                        </div>
                    </div>

                    <!-- Skill Chips -->
                    <div>
                        <h5 class="font-semibold text-gray-800 dark:text-gray-200 mb-3 text-sm md:text-base">Core Technologies</h5>
                        <div class="flex flex-wrap gap-2 md:gap-3">
                            <span class="px-3 py-1.5 rounded-full bg-teal-50 dark:bg-teal-900/20 text-teal-700 dark:text-teal-300 text-xs md:text-sm border border-teal-100 dark:border-teal-800">Laravel</span>
                            <span class="px-3 py-1.5 rounded-full bg-blue-50 dark:bg-blue-900/20 text-blue-700 dark:text-blue-300 text-xs md:text-sm border border-blue-100 dark:border-blue-800">Vue</span>
                            <span class="px-3 py-1.5 rounded-full bg-purple-50 dark:bg-purple-900/20 text-purple-700 dark:text-purple-300 text-xs md:text-sm border border-purple-100 dark:border-purple-800">REST APIs</span>
                            <span class="px-3 py-1.5 rounded-full bg-orange-50 dark:bg-orange-900/20 text-orange-700 dark:text-orange-300 text-xs md:text-sm border border-orange-100 dark:border-orange-800">MySQL</span>
                            <span class="px-3 py-1.5 rounded-full bg-green-50 dark:bg-green-900/20 text-green-700 dark:text-green-300 text-xs md:text-sm border border-green-100 dark:border-green-800">Testing</span>
                            <span class="px-3 py-1.5 rounded-full bg-red-50 dark:bg-red-900/20 text-red-700 dark:text-red-300 text-xs md:text-sm border border-red-100 dark:border-red-800">CI / CD</span>
                            <span class="px-3 py-1.5 rounded-full bg-indigo-50 dark:bg-indigo-900/20 text-indigo-700 dark:text-indigo-300 text-xs md:text-sm border border-indigo-100 dark:border-indigo-800">JavaScript</span>
                            <span class="px-3 py-1.5 rounded-full bg-yellow-50 dark:bg-yellow-900/20 text-yellow-700 dark:text-yellow-300 text-xs md:text-sm border border-yellow-100 dark:border-yellow-800">TypeScript</span>                
                            <span class="px-3 py-1.5 rounded-full bg-gray-50 dark:bg-gray-700 text-gray-700 dark:text-gray-300 text-xs md:text-sm border border-gray-200 dark:border-gray-600">Inertia.js</span>
        

                            <span class="px-3 py-1.5 rounded-full bg-gray-50 dark:bg-gray-700 text-gray-700 dark:text-gray-300 text-xs md:text-sm border border-gray-200 dark:border-gray-600">Tailwind CSS</span>
                        </div>
                    </div>

                    <!-- Action Buttons -->
                    <div class="flex flex-col sm:flex-row gap-3 md:gap-4 pt-2">
                        <a href="/Julfikar Ali_Software_Resume.pdf" target="_blank"
                            class="inline-flex items-center justify-center gap-3 bg-teal-600 hover:bg-teal-700 text-white font-semibold px-6 py-3 rounded-xl shadow-lg transition-all duration-200 transform hover:scale-[1.02] hover:shadow-xl group text-sm md:text-base">
                            <i class="fas fa-download w-4 h-4 md:w-5 md:h-5"></i>
                            Download CV
                        </a>

                        <button @click="scrollToSection('contact')"
                            class="inline-flex items-center justify-center gap-3 border border-teal-600 text-teal-600 dark:text-teal-400 dark:border-teal-400 font-semibold px-6 py-3 rounded-xl hover:bg-teal-50 dark:hover:bg-gray-700 transition-all duration-200 group text-sm md:text-base">
                            <i class="fas fa-envelope w-4 h-4 md:w-5 md:h-5"></i>
                            Contact Me
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </div>
</section>
</template>