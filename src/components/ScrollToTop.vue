<script setup lang="ts">
import { ref, onMounted, onUnmounted } from 'vue';

// State to show/hide button
const isVisible = ref(false);

// Show button after scrolling down 300px
const handleScroll = () => {
    isVisible.value = window.scrollY > 300;
};

// Scroll smoothly to top
const scrollToTop = () => {
    window.scrollTo({ top: 0, behavior: 'smooth' });
};

onMounted(() => {
    window.addEventListener('scroll', handleScroll);
});

onUnmounted(() => {
    window.removeEventListener('scroll', handleScroll);
});
</script>

<template>
    <button v-show="isVisible" @click="scrollToTop"
        class="fixed bottom-8 right-8 bg-teal-500 hover:bg-teal-600 text-white p-3 rounded-full shadow-lg transition-opacity duration-300 z-50 cursor-pointer">
        ↑
    </button>
</template>

<style scoped>
/* Optional: Fade in/out effect */
button[v-cloak] {
    display: none;
}
</style>
