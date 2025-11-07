<template>
    <!-- Footer Section -->
    <footer
        class="bg-gradient-to-br from-gray-50 to-gray-100 dark:from-gray-800 dark:to-gray-900 py-12 transition-colors duration-500">
        <div class="container mx-auto max-w-7xl px-6">
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8 text-center md:text-left">
                <!-- Column 1: About Me -->
                <div class="space-y-4">
                    <h3
                        class="text-xl font-bold text-teal-600 dark:text-teal-400 bg-gradient-to-r from-teal-500 to-teal-600 dark:from-teal-400 dark:to-teal-500 bg-clip-text text-transparent">
                        About Me
                    </h3>
                    <p class="text-gray-600 dark:text-gray-300 leading-relaxed">
                        Hi, I'm Julfikar, a passionate web developer crafting responsive and user-friendly websites.
                        Let's create something amazing together!
                    </p>
                    <div class="pt-2">
                        <span
                            class="inline-flex items-center px-3 py-1 rounded-full text-sm font-medium bg-teal-100 dark:bg-teal-900/30 text-teal-800 dark:text-teal-300">
                            <span class="flex h-2 w-2 relative mr-2">
                                <span
                                    class="animate-ping absolute inline-flex h-full w-full rounded-full bg-teal-400 opacity-75"></span>
                                <span class="relative inline-flex rounded-full h-2 w-2 bg-teal-500"></span>
                            </span>
                            Available for projects
                        </span>
                    </div>
                </div>

                <!-- Column 2: Quick Links -->
                <div class="space-y-4">
                    <h3
                        class="text-xl font-bold text-teal-600 dark:text-teal-400 bg-gradient-to-r from-teal-500 to-teal-600 dark:from-teal-400 dark:to-teal-500 bg-clip-text text-transparent">
                        Quick Links
                    </h3>
                    <ul class="space-y-3 text-gray-600 dark:text-gray-300">
                        <li>
                            <a href="#home"
                                class="group flex items-center justify-center md:justify-start hover:text-teal-600 dark:hover:text-teal-400 transition-all duration-300">
                                <span
                                    class="w-1 h-1 bg-teal-500 rounded-full mr-2 opacity-0 group-hover:opacity-100 transition-opacity duration-300"></span>
                                Home
                            </a>
                        </li>
                        <li>
                            <a href="#about"
                                class="group flex items-center justify-center md:justify-start hover:text-teal-600 dark:hover:text-teal-400 transition-all duration-300">
                                <span
                                    class="w-1 h-1 bg-teal-500 rounded-full mr-2 opacity-0 group-hover:opacity-100 transition-opacity duration-300"></span>
                                About
                            </a>
                        </li>
                        <li>
                            <a href="#projects"
                                class="group flex items-center justify-center md:justify-start hover:text-teal-600 dark:hover:text-teal-400 transition-all duration-300">
                                <span
                                    class="w-1 h-1 bg-teal-500 rounded-full mr-2 opacity-0 group-hover:opacity-100 transition-opacity duration-300"></span>
                                Projects
                            </a>
                        </li>
                        <li>
                            <a href="#contact"
                                class="group flex items-center justify-center md:justify-start hover:text-teal-600 dark:hover:text-teal-400 transition-all duration-300">
                                <span
                                    class="w-1 h-1 bg-teal-500 rounded-full mr-2 opacity-0 group-hover:opacity-100 transition-opacity duration-300"></span>
                                Contact
                            </a>
                        </li>
                    </ul>
                </div>

                <!-- Column 3: Contact Me -->
                <div class="space-y-4">
                    <h3
                        class="text-xl font-bold text-teal-600 dark:text-teal-400 bg-gradient-to-r from-teal-500 to-teal-600 dark:from-teal-400 dark:to-teal-500 bg-clip-text text-transparent">
                        Contact Me
                    </h3>
                    <div class="text-gray-600 dark:text-gray-300 space-y-3">
                        <div class="flex items-center justify-center md:justify-start space-x-2">
                            <i class="fas fa-envelope text-teal-500 dark:text-teal-400 text-sm"></i>
                            <a href="mailto:julfikariucs15@gmail.com"
                                class="hover:text-teal-600 dark:hover:text-teal-400 transition-colors duration-300">
                                julfikariucs15@gmail.com
                            </a>
                        </div>
                        <div class="flex items-center justify-center md:justify-start space-x-2">
                            <i class="fas fa-phone text-teal-500 dark:text-teal-400 text-sm"></i>
                            <a href="tel:+8801521459316"
                                class="hover:text-teal-600 dark:hover:text-teal-400 transition-colors duration-300">
                                +8801521459316
                            </a>
                        </div>
                        <div class="flex items-center justify-center md:justify-start space-x-2">
                            <i class="fas fa-map-marker-alt text-teal-500 dark:text-teal-400 text-sm"></i>
                            <span>Kushtia, Bangladesh</span>
                        </div>
                    </div>
                    <div class="flex justify-center md:justify-start space-x-5 text-2xl pt-2">
                        <a href="https://github.com/julfikariu" target="_blank"
                            class="group text-gray-600 dark:text-gray-400 hover:text-gray-900 dark:hover:text-white transition-all duration-300 transform hover:-translate-y-1">
                            <i class="fab fa-github"></i>
                            <span
                                class="absolute -bottom-8 left-1/2 transform -translate-x-1/2 bg-gray-800 dark:bg-gray-700 text-white text-xs py-1 px-2 rounded opacity-0 group-hover:opacity-100 transition-opacity duration-300 whitespace-nowrap">
                                GitHub
                            </span>
                        </a>
                        <a href="https://linkedin.com/in/julfikar-fsdev" target="_blank"
                            class="group text-gray-600 dark:text-gray-400 hover:text-blue-600 transition-all duration-300 transform hover:-translate-y-1">
                            <i class="fab fa-linkedin"></i>
                            <span
                                class="absolute -bottom-8 left-1/2 transform -translate-x-1/2 bg-gray-800 dark:bg-gray-700 text-white text-xs py-1 px-2 rounded opacity-0 group-hover:opacity-100 transition-opacity duration-300 whitespace-nowrap">
                                LinkedIn
                            </span>
                        </a>
                        <a href="#"
                            class="group text-gray-600 dark:text-gray-400 hover:text-blue-400 transition-all duration-300 transform hover:-translate-y-1">
                            <i class="fab fa-twitter"></i>
                            <span
                                class="absolute -bottom-8 left-1/2 transform -translate-x-1/2 bg-gray-800 dark:bg-gray-700 text-white text-xs py-1 px-2 rounded opacity-0 group-hover:opacity-100 transition-opacity duration-300 whitespace-nowrap">
                                Twitter
                            </span>
                        </a>
                    </div>
                </div>
            </div>

            <div class="mt-12 pt-8 border-t border-gray-300 dark:border-gray-700 text-center">
                <div class="flex flex-col md:flex-row justify-center items-center space-y-4 md:space-y-0">
                    <p class="text-gray-500 dark:text-gray-400 text-sm">
                        &copy; 2024 Julfikar Ali. All rights reserved.
                    </p>
                </div>
            </div>
        </div>
    </footer>
</template>