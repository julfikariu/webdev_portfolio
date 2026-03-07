<script setup lang="ts">
import { ref, onMounted, onUnmounted, watch } from 'vue';

const darkMode = ref<boolean>(true);
const activeSection = ref<string>('home'); // track active menu

function setDocumentTheme(isDark: boolean) {
    if (isDark) document.documentElement.classList.add('dark');
    else document.documentElement.classList.remove('dark');
}

function toggleTheme() {
    darkMode.value = !darkMode.value;
}

watch(darkMode, (val) => {
    setDocumentTheme(val);
    try {
        localStorage.setItem('theme', val ? 'dark' : 'light');
    } catch { }
}, { immediate: false });

onMounted(() => {
    let savedTheme: string | null = null;
    try { savedTheme = localStorage.getItem('theme'); } catch { }
    if (savedTheme === 'dark') darkMode.value = true;
    else if (savedTheme === 'light') darkMode.value = false;
    else darkMode.value = true;

    setDocumentTheme(darkMode.value);

    window.addEventListener('scroll', handleScroll);
});

onUnmounted(() => {
    window.removeEventListener('scroll', handleScroll);
});

// Smooth scroll
const scrollToSection = (id: string) => {
    const element = document.getElementById(id);
    if (element) {
        const yOffset = -80; // offset for fixed header
        const y = element.getBoundingClientRect().top + window.pageYOffset + yOffset;
        window.scrollTo({ top: y, behavior: 'smooth' });
    }
};

// Update active menu based on scroll
const handleScroll = () => {
    const sections = ['home', 'about', 'experience', 'skills', 'projects', 'education', 'contact'];
    const scrollPos = window.scrollY + 100; // small offset for header
    for (const id of sections) {
        const el = document.getElementById(id);
        if (el) {
            const top = el.offsetTop;
            const bottom = top + el.offsetHeight;
            if (scrollPos >= top && scrollPos < bottom) {
                activeSection.value = id;
            }
        }
    }
};
</script>

<template>
    <header class="fixed w-full top-0 z-50 h-18 bg-gray-100 dark:bg-gray-900 bg-opacity-80 backdrop-blur-sm shadow-sm">
        <nav class="container mx-auto max-w-7xl px-6 py-4 flex items-center justify-between">
            <!-- Logo -->
            <a href="/" class="text-2xl font-bold text-teal-400">&lt;JA&gt;</a>

            <!-- Desktop Menu -->
            <ul class="hidden md:flex items-center space-x-6 font-semibold">
                <li>
                    <button @click="scrollToSection('home')"
                        :class="activeSection === 'home' ? 'text-teal-400' : 'text-gray-700 dark:text-gray-300'"
                        class="hover:text-teal-400 cursor-pointer transition-colors duration-300">Home</button>
                </li>
                <li>
                    <button @click="scrollToSection('about')"
                        :class="activeSection === 'about' ? 'text-teal-400' : 'text-gray-700 dark:text-gray-300'"
                        class="hover:text-teal-400 cursor-pointer transition-colors duration-300">About</button>
                </li>
                <li>
                    <button @click="scrollToSection('experience')"
                        :class="activeSection === 'experience' ? 'text-teal-400' : 'text-gray-700 dark:text-gray-300'"
                        class="hover:text-teal-400 cursor-pointer transition-colors duration-300">Experience</button>
                </li>
                <li>
                    <button @click="scrollToSection('skills')"
                        :class="activeSection === 'skills' ? 'text-teal-400' : 'text-gray-700 dark:text-gray-300'"
                        class="hover:text-teal-400 cursor-pointer transition-colors duration-300">Skills</button>
                </li>
                <li>
                    <button @click="scrollToSection('projects')"
                        :class="activeSection === 'projects' ? 'text-teal-400' : 'text-gray-700 dark:text-gray-300'"
                        class="hover:text-teal-400 cursor-pointer transition-colors duration-300">Projects</button>
                </li>
                <li>
                    <button @click="scrollToSection('education')"
                        :class="activeSection === 'education' ? 'text-teal-400' : 'text-gray-700 dark:text-gray-300'"
                        class="hover:text-teal-400 cursor-pointer transition-colors duration-300">Education</button>
                </li>
                <li>
                    <button @click="scrollToSection('contact')"
                        :class="activeSection === 'contact' ? 'text-teal-400' : 'text-gray-700 dark:text-gray-300'"
                        class="hover:text-teal-400 cursor-pointer transition-colors duration-300">Contact</button>
                </li>

                <!-- Dark Mode Toggle -->
                <li>
                    <button @click="toggleTheme" class="focus:outline-none cursor-pointer"
                        :title="darkMode ? 'Switch to light' : 'Switch to dark'">
                        <i
                            :class="[darkMode ? 'fas fa-moon' : 'fas fa-sun', 'text-xl', 'text-yellow-400', 'hover:text-yellow-300', 'transition-colors', 'duration-200']"></i>
                    </button>
                </li>
            </ul>

            <!-- Mobile Menu Button -->
            <div class="flex items-center md:hidden space-x-4">
                <button @click="toggleTheme" class="focus:outline-none cursor-pointer"
                    :title="darkMode ? 'Switch to light' : 'Switch to dark'">
                    <i
                        :class="[darkMode ? 'fas fa-moon' : 'fas fa-sun', 'text-xl', 'text-yellow-400', 'hover:text-yellow-300', 'transition-colors', 'duration-300']"></i>
                </button>
            </div>
        </nav>
    </header>
</template>
