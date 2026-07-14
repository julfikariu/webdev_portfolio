<template>
    <span aria-live="polite" class="whitespace-nowrap">{{ displayText }}</span>
    <span aria-hidden="true" class="ml-1 text-gray-500 dark:text-gray-400 select-none animate-pulse">|</span>
</template>

<script setup lang="ts">
import { ref, onMounted, onBeforeUnmount } from 'vue';

interface Props {
  phrases?: string[];
  typingSpeed?: number;
  deletingSpeed?: number;
  pause?: number;
  loop?: boolean;
  startIndex?: number;
}

// use withDefaults() instead of inline type+object
const props = withDefaults(defineProps<Props>(), {
  phrases: () => ['Full-Stack Engineer', 'Systems Architect', 'Database Optimization Expert', 'Vue & Laravel Specialist'],
  typingSpeed: 120,
  deletingSpeed: 60,
  pause: 1400,
  loop: true,
  startIndex: 0
});

const displayText = ref('');
let phraseIndex = props.startIndex;
let charIndex = 0;
let isDeleting = false;
let timerId: number | null = null;

function clearTimer() {
  if (timerId !== null) {
    clearTimeout(timerId);
    timerId = null;
  }
}

function schedule(fn: () => void, delay: number) {
  clearTimer();
  timerId = window.setTimeout(fn, delay);
}

function tick() {
  const phrases = props.phrases;
  if (!phrases.length) return;

  const current = phrases[phraseIndex % phrases.length];

  if (!isDeleting) {
    charIndex = Math.min(current.length, charIndex + 1);
    displayText.value = current.slice(0, charIndex);

    if (charIndex < current.length) {
      schedule(tick, props.typingSpeed);
    } else {
      if (props.loop || phraseIndex < phrases.length - 1) {
        isDeleting = true;
        schedule(tick, props.pause);
      }
    }
  } else {
    charIndex = Math.max(0, charIndex - 1);
    displayText.value = current.slice(0, charIndex);

    if (charIndex > 0) {
      schedule(tick, props.deletingSpeed);
    } else {
      isDeleting = false;
      phraseIndex = (phraseIndex + 1) % phrases.length;
      schedule(tick, 300);
    }
  }
}

onMounted(() => {
  schedule(tick, 300);
});

onBeforeUnmount(() => {
  clearTimer();
});
</script>
