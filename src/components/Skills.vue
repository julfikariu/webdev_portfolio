<script setup lang="ts">
import { ref } from 'vue';

const skillCategories = ref([
    {
        title: 'Backend Architecture',
        skills: [
            { name: 'Laravel (Ecosystem)', highlight: true },
            { name: 'PHP (Core, OOP)', highlight: true },
            { name: 'Node.js', highlight: false },
            { name: 'CakePHP', highlight: false },
            { name: 'RESTful API Design', highlight: true }
        ]
    },
    {
        title: 'Frontend Engineering',
        skills: [
            { name: 'Vue.js (Vue 3, Composition API)', highlight: true },
            { name: 'React.js', highlight: true },
            { name: 'TypeScript', highlight: true },
            { name: 'JavaScript (ES6+)', highlight: true },
            { name: 'Tailwind CSS', highlight: false },
            { name: 'HTML5 & CSS3', highlight: false }
        ]
    },
    {
        title: 'Database & Performance',
        skills: [
            { name: 'MySQL Optimization', highlight: true },
            { name: 'Database Architecture', highlight: true },
            { name: 'Redis / Caching', highlight: false },
            { name: 'Complex Aggregations', highlight: true }
        ]
    },
    {
        title: 'Infrastructure & DevOps',
        skills: [
            { name: 'Docker', highlight: true },
            { name: 'CI/CD Pipelines (GitHub Actions)', highlight: true },
            { name: 'AWS (EC2)', highlight: false },
            { name: 'Linux Server Administration', highlight: true },
            { name: 'Git Architecture', highlight: false }
        ]
    }
]);
</script>

<template>
    <section id="skills" class="py-20 bg-gray-100 dark:bg-gray-900 transition-colors duration-300">
        <div class="container mx-auto max-w-7xl px-6">
            <h2 class="text-3xl md:text-4xl font-extrabold text-center text-teal-500 dark:text-teal-400 mb-4 tracking-tight">
                Engineering Expertise
            </h2>
            <div class="w-24 h-1 bg-teal-500 mx-auto mb-16 rounded-full"></div>

            <div class="grid md:grid-cols-2 gap-10">
                <div v-for="(category, index) in skillCategories" :key="index"
                     class="bg-white dark:bg-gray-800 p-8 rounded-3xl shadow-xl border border-gray-200 dark:border-gray-700 hover:border-teal-500 transition-colors duration-300 transform hover:-translate-y-1">
                    <h3 class="text-2xl font-bold text-gray-900 dark:text-white mb-6 border-b border-gray-200 dark:border-gray-700 pb-3">
                        {{ category.title }}
                    </h3>
                    <ul class="space-y-3 text-gray-700 dark:text-gray-300">
                        <li v-for="(skill, sIndex) in category.skills" :key="sIndex" class="flex items-center">
                            <span class="w-2 h-2 bg-teal-500 dark:bg-teal-400 rounded-full mr-3 flex-shrink-0 shadow-[0_0_8px_rgba(45,212,191,0.5)]"></span>
                            <strong v-if="skill.highlight" class="font-semibold">{{ skill.name }}</strong>
                            <template v-else>{{ skill.name }}</template>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </section>
</template>