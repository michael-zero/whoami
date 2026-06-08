<template>
  <header class="bg-primary px-6 py-5">
    <nav>
      <RouterLink to="/" class="text-ice hover:text-secondary transition-colors">
        Home
      </RouterLink>
    </nav>
  </header>
</template>

<script setup lang="ts">
import { RouterLink } from 'vue-router'
</script>
