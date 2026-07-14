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
                                Software Engineer - Flick Media Ltd
                            </h4>
                            <p class="text-sm font-light text-gray-500 dark:text-gray-400">Jul 2025 - Jun 2026 | Khulna, Bangladesh</p>
                            <ul class="list-disc list-inside text-gray-600 dark:text-gray-300 space-y-1">
                                <li>Architected a multi-tenant SaaS HRM system from the ground up using Laravel, Inertia.js, Vue 3, TypeScript, and TailwindCSS; delivered staff management, leave workflows, training modules, account impersonation, and full tenant isolation.</li>
                                <li>Contributed to development and maintenance of a Property Management System in CodeIgniter — tenancy lifecycle, estate-agent workflows, mortgage tracking, insurance, automated reminders, and transaction history.</li>
                                <li>Built a cross-platform desktop time-tracker with Rust, Vue 3, and Tauri modelled on the Upwork client; added background keystroke/mouse activity counters, multiplatform packaging, and local SQLite persistence.</li>
                                <li>Accelerated team feature delivery by embedding Cursor AI into the workflow, shortening prototyping and debugging cycles.</li>
                            </ul>
                        </div>
                        <div class="border-l-4 border-gray-300 dark:border-gray-600 pl-6 space-y-2">
                            <h4 class="text-xl font-bold text-teal-600 dark:text-teal-400">
                                Software Engineer - Tiger Tech Co., Ltd.
                            </h4>
                            <p class="text-sm font-light text-gray-500 dark:text-gray-400">Feb 2023 - Jun 2025 | Tokyo, Japan — Remote</p>
                            <ul class="list-disc list-inside text-gray-600 dark:text-gray-300 space-y-1">
                                <li>Integrated 3D Secure (3DS2) via Veritrans.jp on a high-volume B2B platform, enabling PCI-compliant credit card processing and chargeback risk mitigation.</li>
                                <li>Architected a Single Sign-On (SSO) solution consolidating authentication across multiple enterprise applications and standardising session security policy.</li>
                                <li>Provisioned production infrastructure on AWS EC2 with Apache, MySQL, and Laravel — server hardening, deployment automation, and staging/production environment parity.</li>
                                <li>Implemented OAuth social login (Google, Microsoft) and authored RESTful APIs in Laravel consumed by frontend clients and third-party authentication workflows.</li>
                                <li>Authored unit test suites covering payment and authentication flows, eliminating post-deployment regressions on critical transaction paths.</li>
                            </ul>
                        </div>
                        <!-- Experience Item 2 -->
                        <div class="border-l-4 border-gray-300 dark:border-gray-600 pl-6 space-y-2">
                            <h4 class="text-xl font-bold text-teal-600 dark:text-teal-400">
                                Software Engineer - XOR Software Solutions
                            </h4>
                            <p class="text-sm font-light text-gray-500 dark:text-gray-400">Oct 2021 - Jan 2023 | Khulna, Bangladesh</p>
                            <ul class="list-disc list-inside text-gray-600 dark:text-gray-300 space-y-1">
                                <li>Delivered full-stack implementations across Job Portal, E-commerce, B2B/B2C marketplace, and Ticketing verticals — end-to-end from schema design to production UI.</li>
                                <li>Architected a secure API layer using Laravel Passport (OAuth2), enforcing token-based authentication across consumer and partner integrations.</li>
                                <li>Engineered core LMS modules for course creation, enrolment, progress tracking, and content management with multi-role access for instructors, learners, and admins.</li>
                                <li>Optimised complex MySQL queries via Laravel Eloquent ORM, improving response times on high-traffic reporting and search endpoints.</li>
                            </ul>
                        </div>
                        <!-- Experience Item 3 -->
                        <div class="border-l-4 border-gray-300 dark:border-gray-600 pl-6 space-y-2">
                            <h4 class="text-xl font-bold text-teal-600 dark:text-teal-400">
                                Web Application Developer - BDCODER Software
                            </h4>
                            <p class="text-sm font-light text-gray-500 dark:text-gray-400">Apr 2021 - Sep 2021 | Khulna, Bangladesh — Remote</p>
                            <ul class="list-disc list-inside text-gray-600 dark:text-gray-300 space-y-1">
                                <li>Developed business-critical CMS platforms with integrated RESTful APIs and configurable content management workflows.</li>
                                <li>Enhanced platform security by integrating Google reCAPTCHA, live chat, and AJAX real-time search, reducing bot-driven form abuse.</li>
                                <li>Produced complete technical documentation including user manuals, system specifications, and operational runbooks for delivered systems.</li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

</template>