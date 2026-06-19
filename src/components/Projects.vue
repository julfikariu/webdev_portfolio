<script setup lang="ts">
import { ref } from 'vue';

const projects = ref([
    {
        title: 'HRM SaaS Platform',
        situation: 'Organizations struggled with fragmented HR processes, manual attendance tracking, and lack of centralized scheduling.',
        task: 'Architect a scalable, multi-tenant SaaS application to centralize workforce management, subscription billing, and role-based access for diverse organizations.',
        action: 'Developed a robust Laravel/Vue.js architecture utilizing Inertia.js for seamless SPA navigation. Implemented automated notification pipelines, secure document management, and modular role-based access controls.',
        result: 'Delivered a highly performant platform that reduced HR manual workload by streamlining operations and automating critical workflows like leave approvals and scheduling.',
        tech: ['Laravel', 'Vue.js', 'Inertia.js', 'Tailwind CSS', 'MySQL'],
        image: '/img/hrm_dashboard.png',
        liveLink: '#',
        detailsLink: '/project-details/hrm-saas',
        isReverse: false
    },
    {
        title: 'E-Commerce Synchronization Engine',
        situation: 'A retail business required a modern, scalable online storefront with a robust admin panel capable of managing large product catalogs and tracking orders.',
        task: 'Build a secure, full-stack e-commerce application handling everything from user registration to complex product categorizations and order lifecycle management.',
        action: 'Designed a high-performance database schema in MySQL to handle complex aggregations. Built a RESTful backend using Laravel to sync product APIs and utilized jQuery/Bootstrap for dynamic, responsive frontend interactions.',
        result: 'Created a highly responsive shopping experience with seamless checkout flows, enabling efficient inventory tracking and accelerating order processing.',
        tech: ['Laravel', 'MySQL DB', 'jQuery', 'Bootstrap', 'JavaScript', 'HTML/CSS'],
        image: 'https://placehold.co/300x200/222222/a3e635?text=E-Commerce',
        liveLink: '#',
        sourceLink: '#',
        isReverse: true
    },
    {
        title: 'LMS with Secure Payment Gateways',
        situation: 'Instructors lacked a streamlined platform to monetize their courses with secure, integrated payment processing.',
        task: 'Engineer a lightweight Learning Management System supporting distinct instructor/student roles, course browsing, and secure transaction flows.',
        action: 'Implemented secure authentication models and integrated third-party payment APIs (PayPal, Stripe) within a custom PHP/Laravel backend to handle transactional integrity.',
        result: 'Successfully launched a monetization channel for tutors, ensuring secure and reliable course purchases with zero transaction drops.',
        tech: ['Laravel', 'PHP', 'MySQL DB', 'JavaScript', 'HTML/CSS'],
        image: 'https://placehold.co/200x100/222222/a3e635?text=LMS',
        liveLink: '#',
        sourceLink: '#',
        isReverse: false
    },
    {
        title: 'Helpdesk Automation & Tracking System',
        situation: 'Contest administrators needed a way to dynamically track and analyze user performance across multiple disparate online judges.',
        task: 'Develop an automated data pipeline to ingest performance metrics and provide actionable insights into user achievements.',
        action: 'Engineered a backend system in Laravel that consumes REST APIs from external judges, aggregating data and evaluating complex performance metrics in real-time.',
        result: 'Provided an automated, insightful dashboard that eliminated manual tracking, significantly improving the evaluation process for administrators.',
        tech: ['Laravel', 'PHP', 'REST API', 'Bootstrap'],
        image: 'https://placehold.co/600x400/222222/a3e635?text=Helpdesk',
        liveLink: '#',
        sourceLink: '#',
        isReverse: true
    }
]);
</script>

<template>
    <section id="projects" class="bg-gradient-to-br py-20 bg-gray-100 dark:from-gray-800 dark:to-gray-900 transition-colors duration-300">
        <div class="container mx-auto max-w-7xl px-6">
            <h2 class="text-3xl md:text-4xl font-bold text-center text-teal-500 dark:text-teal-400 mb-12">
                Engineering Case Studies
            </h2>

            <!-- Project Cards Loop -->
            <div v-for="(project, index) in projects" :key="index"
                 class="bg-white dark:bg-gray-800 rounded-3xl shadow-xl border border-gray-200 dark:border-gray-700 overflow-hidden mb-12 md:flex transform hover:-translate-y-2 transition-all duration-300">
                
                <!-- Image Container -->
                <div class="md:w-1/2 flex items-center justify-center p-6 bg-gray-50 dark:bg-gray-800/50"
                     :class="project.isReverse ? 'order-1 md:order-2' : ''">
                    <img :src="project.image" :alt="project.title" class="rounded-2xl w-full max-h-80 object-cover shadow-md">
                </div>
                
                <!-- Content Container -->
                <div class="md:w-1/2 p-8 md:p-12"
                     :class="project.isReverse ? 'order-2 md:order-1' : ''">
                    <h3 class="text-2xl font-bold text-gray-900 dark:text-white mb-6">{{ project.title }}</h3>
                    
                    <div class="space-y-4 mb-8">
                        <div>
                            <strong class="text-teal-600 dark:text-teal-400 text-sm uppercase tracking-wide">Situation:</strong>
                            <p class="text-gray-700 dark:text-gray-300 mt-1">{{ project.situation }}</p>
                        </div>
                        <div>
                            <strong class="text-teal-600 dark:text-teal-400 text-sm uppercase tracking-wide">Task:</strong>
                            <p class="text-gray-700 dark:text-gray-300 mt-1">{{ project.task }}</p>
                        </div>
                        <div>
                            <strong class="text-teal-600 dark:text-teal-400 text-sm uppercase tracking-wide">Action:</strong>
                            <p class="text-gray-700 dark:text-gray-300 mt-1">{{ project.action }}</p>
                        </div>
                        <div>
                            <strong class="text-teal-600 dark:text-teal-400 text-sm uppercase tracking-wide">Result:</strong>
                            <p class="text-gray-700 dark:text-gray-300 mt-1 font-medium">{{ project.result }}</p>
                        </div>
                    </div>

                    <div class="flex flex-wrap gap-2 mb-8">
                        <span v-for="(tech, tIndex) in project.tech" :key="tIndex" 
                              class="bg-gray-100 dark:bg-gray-700 text-gray-700 dark:text-gray-300 py-1.5 px-4 rounded-full text-xs font-semibold border border-gray-200 dark:border-gray-600">
                            {{ tech }}
                        </span>
                    </div>

                    <div class="flex flex-col sm:flex-row space-y-3 sm:space-y-0 sm:space-x-4">
                        <a v-if="project.liveLink" :href="project.liveLink" class="bg-teal-600 text-white font-semibold py-2.5 px-6 rounded-xl text-sm hover:bg-teal-700 transition-colors duration-300 text-center shadow-lg hover:shadow-xl">Live Site</a>
                        <a v-if="project.detailsLink" :href="project.detailsLink" class="bg-gray-100 dark:bg-gray-700 text-gray-700 dark:text-gray-300 border border-gray-200 dark:border-gray-600 font-semibold py-2.5 px-6 rounded-xl text-sm hover:bg-gray-200 dark:hover:bg-gray-600 transition-colors duration-300 text-center">View Details</a>
                        <a v-if="project.sourceLink" :href="project.sourceLink" class="bg-gray-100 dark:bg-gray-700 text-gray-700 dark:text-gray-300 border border-gray-200 dark:border-gray-600 font-semibold py-2.5 px-6 rounded-xl text-sm hover:bg-gray-200 dark:hover:bg-gray-600 transition-colors duration-300 text-center">Source Code</a>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>