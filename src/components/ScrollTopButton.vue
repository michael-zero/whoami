<template>
  <button @click="scrollToTop"
          class="fixed bottom-6 right-6 z-50 w-10 h-10 flex items-center justify-center rounded-full border border-zinc-700 text-gray-custom hover:text-secondary hover:border-secondary bg-primary transition-all duration-300"
          :class="visible ? 'opacity-100 pointer-events-auto' : 'opacity-0 pointer-events-none'">
    <span class="text-lg leading-none">↑</span>
  </button>
</template>

<script setup lang="ts">
import { ref, onMounted, onUnmounted } from 'vue'

const visible = ref(false)

function onScroll() {
  visible.value = window.scrollY > 300
}

function scrollToTop() {
  window.scrollTo({ top: 0, behavior: 'smooth' })
}

onMounted(() => window.addEventListener('scroll', onScroll))
onUnmounted(() => window.removeEventListener('scroll', onScroll))
</script>
