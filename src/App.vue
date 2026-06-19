<script setup lang="ts">
import Footer from '@components/Footer.vue';
import Header from '@components/Header.vue';
import ScrollToTop from '@components/ScrollToTop.vue';
</script>

<template>
    <Header />
    <router-view />
    <Footer />
    <ScrollToTop />
</template>

<style scoped>

</style>
