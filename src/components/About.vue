<script lang="ts">


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
                <!-- Profile Section -->
                <div class="flex flex-col items-center lg:items-start space-y-6">
                    <!-- Avatar Container -->
                    <div class="relative group">
                        <div class="w-32 h-32 md:w-40 md:h-40 rounded-2xl flex items-center justify-center bg-gradient-to-br from-teal-500 to-teal-300 dark:from-teal-600 dark:to-teal-400 shadow-lg transform transition-all duration-300 group-hover:scale-105 group-hover:shadow-xl">
                            <svg width="64" height="64" viewBox="0 0 100 100" aria-hidden="true" class="text-white md:w-16 md:h-16">
                                <rect width="100" height="100" rx="18" fill="currentColor" opacity="0.06" />
                                <text x="50%" y="52%" dominant-baseline="middle" text-anchor="middle" font-size="34"
                                    font-weight="700" fill="white"
                                    font-family="Inter, ui-sans-serif, system-ui, -apple-system, 'Segoe UI', Roboto">
                                    J A
                                </text>
                            </svg>
                        </div>
                        <!-- Status Indicator -->
                        <div class="absolute -bottom-2 -right-2 w-6 h-6 bg-green-500 dark:bg-green-400 rounded-full border-4 border-white dark:border-gray-800">
                            <span class="sr-only">Available for work</span>
                        </div>
                    </div>

                    <!-- Personal Info -->
                    <div class="text-center lg:text-left space-y-3">
                        <div>
                            <h3 class="text-xl font-bold text-gray-900 dark:text-white">Julfikar Ali</h3>
                            <p class="text-sm text-gray-600 dark:text-gray-300 mt-1">Full Stack Web Developer</p>
                            <p class="text-xs text-teal-600 dark:text-teal-400 font-medium mt-1">Laravel & React.js Specialist</p>
                        </div>

                        <!-- Contact Buttons -->
                        <div class="flex flex-col sm:flex-row lg:flex-col gap-3 pt-2">
                            <a href="mailto:julfikariucs15@gmail.com"
                                class="inline-flex items-center justify-center gap-2 text-sm font-medium px-4 py-2 rounded-xl border border-gray-200 dark:border-gray-600 bg-gray-50 dark:bg-gray-700 hover:bg-gray-100 dark:hover:bg-gray-600 transition-all duration-200 group min-w-0">
                                <svg class="w-4 h-4 text-teal-600 dark:text-teal-400 flex-shrink-0" viewBox="0 0 24 24" fill="none" stroke="currentColor">
                                    <path d="M3 8.5v7A2.5 2.5 0 0 0 5.5 18h13A2.5 2.5 0 0 0 21 15.5v-7"
                                        stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                                </svg>
                                <span class="truncate">julfikariucs15@gmail.com</span>
                            </a>

                            <a href="tel:+8801521459316"
                                class="inline-flex items-center justify-center gap-2 text-sm font-medium px-4 py-2 rounded-xl border border-gray-200 dark:border-gray-600 bg-gray-50 dark:bg-gray-700 hover:bg-gray-100 dark:hover:bg-gray-600 transition-all duration-200 group min-w-0">
                                <svg class="w-4 h-4 text-teal-600 dark:text-teal-400 flex-shrink-0" viewBox="0 0 24 24" fill="none" stroke="currentColor">
                                    <path
                                        d="M22 16.92V21a1 1 0 0 1-1.11 1A19 19 0 0 1 3 5.11 1 1 0 0 1 4 4h4.09a1 1 0 0 1 1 .75c.12.66.37 1.3.73 1.84l-.27.27a16 16 0 0 0 6.36 6.36l.27-.27c.54.36 1.18.61 1.84.73a1 1 0 0 1 .75 1V21z"
                                        stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                                </svg>
                                <span class="truncate">+8801521459316</span>
                            </a>
                        </div>
                    </div>
                </div>

                <!-- Content Section -->
                <div class="lg:col-span-2 space-y-6 md:space-y-8">
                    <!-- Introduction -->
                    <div>
                        <h4 class="text-xl md:text-2xl font-bold text-gray-900 dark:text-white mb-4">
                            Hello, I'm Julfikar Ali
                        </h4>

                        <p class="text-gray-600 dark:text-gray-300 leading-relaxed md:leading-loose text-sm md:text-base">
                            I'm a professional and passionate web developer with over 4 years of experience building
                            scalable, maintainable web applications. My main focus is crafting high-performance solutions using
                            Laravel for backend and React for frontend, combined with strong database design (MySQL) and clean,
                            testable code. I love turning ideas into production-ready products and continuously improving through
                            learning and collaboration.
                        </p>
                    </div>

                    <!-- Quick Highlights Grid -->
                    <div class="grid grid-cols-1 sm:grid-cols-2 gap-4 md:gap-6">
                        <div class="bg-gray-50 dark:bg-gray-700/50 p-4 rounded-xl border border-gray-100 dark:border-gray-600">
                            <p class="font-semibold text-gray-800 dark:text-gray-100 text-sm md:text-base">Experience</p>
                            <p class="text-gray-500 dark:text-gray-300 text-sm mt-1">4+ years building web apps</p>
                        </div>
                        <div class="bg-gray-50 dark:bg-gray-700/50 p-4 rounded-xl border border-gray-100 dark:border-gray-600">
                            <p class="font-semibold text-gray-800 dark:text-gray-100 text-sm md:text-base">Location</p>
                            <p class="text-gray-500 dark:text-gray-300 text-sm mt-1">Kushtia, Bangladesh</p>
                        </div>
                        <div class="bg-gray-50 dark:bg-gray-700/50 p-4 rounded-xl border border-gray-100 dark:border-gray-600">
                            <p class="font-semibold text-gray-800 dark:text-gray-100 text-sm md:text-base">Primary Stack</p>
                            <p class="text-gray-500 dark:text-gray-300 text-sm mt-1">Laravel • React • MySQL</p>
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
                            <span class="px-3 py-1.5 rounded-full bg-blue-50 dark:bg-blue-900/20 text-blue-700 dark:text-blue-300 text-xs md:text-sm border border-blue-100 dark:border-blue-800">React</span>
                            <span class="px-3 py-1.5 rounded-full bg-purple-50 dark:bg-purple-900/20 text-purple-700 dark:text-purple-300 text-xs md:text-sm border border-purple-100 dark:border-purple-800">REST APIs</span>
                            <span class="px-3 py-1.5 rounded-full bg-orange-50 dark:bg-orange-900/20 text-orange-700 dark:text-orange-300 text-xs md:text-sm border border-orange-100 dark:border-orange-800">MySQL</span>
                            <span class="px-3 py-1.5 rounded-full bg-green-50 dark:bg-green-900/20 text-green-700 dark:text-green-300 text-xs md:text-sm border border-green-100 dark:border-green-800">Testing</span>
                            <span class="px-3 py-1.5 rounded-full bg-red-50 dark:bg-red-900/20 text-red-700 dark:text-red-300 text-xs md:text-sm border border-red-100 dark:border-red-800">CI / CD</span>
                            <span class="px-3 py-1.5 rounded-full bg-indigo-50 dark:bg-indigo-900/20 text-indigo-700 dark:text-indigo-300 text-xs md:text-sm border border-indigo-100 dark:border-indigo-800">JavaScript</span>
                            <span class="px-3 py-1.5 rounded-full bg-gray-50 dark:bg-gray-700 text-gray-700 dark:text-gray-300 text-xs md:text-sm border border-gray-200 dark:border-gray-600">Tailwind CSS</span>
                        </div>
                    </div>

                    <!-- Action Buttons -->
                    <div class="flex flex-col sm:flex-row gap-3 md:gap-4 pt-2">
                        <a href="/Julfikar_Ali_CV.pdf"
                            class="inline-flex items-center justify-center gap-3 bg-teal-600 hover:bg-teal-700 text-white font-semibold px-6 py-3 rounded-xl shadow-lg transition-all duration-200 transform hover:scale-[1.02] hover:shadow-xl group text-sm md:text-base">
                            <svg class="w-4 h-4 md:w-5 md:h-5" viewBox="0 0 24 24" fill="none" stroke="currentColor">
                                <path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4" stroke-width="1.5"
                                    stroke-linecap="round" stroke-linejoin="round" />
                                <path d="M7 10l5 5 5-5" stroke-width="1.5" stroke-linecap="round"
                                    stroke-linejoin="round" />
                                <path d="M12 15V3" stroke-width="1.5" stroke-linecap="round"
                                    stroke-linejoin="round" />
                            </svg>
                            Download CV
                        </a>

                        <a href="#contact"
                            class="inline-flex items-center justify-center gap-3 border border-teal-600 text-teal-600 dark:text-teal-400 dark:border-teal-400 font-semibold px-6 py-3 rounded-xl hover:bg-teal-50 dark:hover:bg-gray-700 transition-all duration-200 group text-sm md:text-base">
                            <svg class="w-4 h-4 md:w-5 md:h-5" viewBox="0 0 24 24" fill="none" stroke="currentColor">
                                <path d="M21 11.5a8.38 8.38 0 0 1-.9 3.8 8.5 8.5 0 0 1-7.6 4.7 8.38 8.38 0 0 1-3.8-.9L3 21l1.9-5.7a8.38 8.38 0 0 1-.9-3.8 8.5 8.5 0 0 1 4.7-7.6 8.38 8.38 0 0 1 3.8-.9h.5a8.48 8.48 0 0 1 8 8v.5z"
                                    stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round" />
                            </svg>
                            Contact Me
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</section>
</template>