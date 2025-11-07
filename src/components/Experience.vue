<script setup lang="ts">
</script>

<template>
    <!-- Experience Section -->
    <section id="experience" class="py-20 bg-gray-100 dark:bg-gray-900 transition-colors duration-300">
        <div class="container mx-auto max-w-7xl px-6">
            <h2 class="text-2xl md:text-4xl font-extrabold text-center text-teal-400 mb-4 tracking-tight">
            My Experience
        </h2>
        <div class="w-24 h-1 bg-teal-500 mx-auto mb-16 rounded-full"></div>
            <div class="space-y-12">
                <!-- Work Experience -->
                <div
                    class="bg-white dark:bg-gray-800 p-8 rounded-3xl shadow-xl border-t-4 border-teal-500 transition-colors duration-300">
                    <h3 class="text-2xl font-semibold text-gray-900 dark:text-white mb-4">
                        Work Experience
                    </h3>
                    <div class="space-y-6">
                        <!-- Experience Item 1 -->
                        <div class="border-l-4 border-gray-300 dark:border-gray-600 pl-6 space-y-2">
                            <h4 class="text-xl font-bold text-teal-600 dark:text-teal-400">
                                Software Engineer - Tiger Tech Co,Ltd.
                            </h4>
                            <p class="text-sm font-light text-gray-500 dark:text-gray-400">Feb 2023 - Jun 2025</p>
                            <ul class="list-disc list-inside text-gray-600 dark:text-gray-300 space-y-1">
                                <li>Implemented 3D Secure payment gateway using Veritrans.jp for secure B2B
                                    transactions.</li>
                                <li>Developed a Single Sign-On (SSO) solution to enhance security and streamline user
                                    logins.</li>
                                <li>Managed server setup and optimization on AWS EC2 using Apache, MySQL, and Laravel.
                                </li>
                                <li>Implemented social login integrations (Google, Microsoft, Apple) and RESTful APIs in
                                    Laravel.</li>
                                <li>Wrote unit tests to ensure robust and bug-free features.</li>
                            </ul>
                        </div>
                        <!-- Experience Item 2 -->
                        <div class="border-l-4 border-gray-300 dark:border-gray-600 pl-6 space-y-2">
                            <h4 class="text-xl font-bold text-teal-600 dark:text-teal-400">
                                Software Engineer - XOR Software Solutions
                            </h4>
                            <p class="text-sm font-light text-gray-500 dark:text-gray-400">Oct 2021 - Jan 2023</p>
                            <ul class="list-disc list-inside text-gray-600 dark:text-gray-300 space-y-1">
                                <li>Served as a Full Stack Web Developer, managing both backend and frontend tasks.</li>
                                <li>Utilized Laravel Eloquent ORM for data storage and querying from a MySQL database.
                                </li>
                                <li>Developed secure RESTful APIs with Laravel Passport for user authentication.</li>
                                <li>Implemented course creation and management features in a Learning Management System
                                    (LMS).</li>
                            </ul>
                        </div>
                        <!-- Experience Item 3 -->
                        <div class="border-l-4 border-gray-300 dark:border-gray-600 pl-6 space-y-2">
                            <h4 class="text-xl font-bold text-teal-600 dark:text-teal-400">
                                Laravel Web Application Developer - BDCODER Software
                            </h4>
                            <p class="text-sm font-light text-gray-500 dark:text-gray-400">Apr 2021 - Sep 2021</p>
                            <ul class="list-disc list-inside text-gray-600 dark:text-gray-300 space-y-1">
                                <li>Developed and implemented backend applications and RESTful APIs based on client
                                    requirements.</li>
                                <li>Enhanced user experience and security by integrating Google reCAPTCHA, live chat,
                                    and AJAX search.</li>
                                <li>Created system documentation including user manuals and technical specifications.
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

</template>