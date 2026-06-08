<template>
  <main class="bg-primary">
    <HeroSection />
    <SobreSection />
    <TechStackSection />
    <ExperienciaSection />
    <MentoriaSection />
  </main>
  <AppFooter />
</template>

<script setup lang="ts">
import AppFooter from '@/components/AppFooter.vue'
import HeroSection from '@/components/HeroSection.vue'
import SobreSection from '@/components/SobreSection.vue'
import TechStackSection from '@/components/TechStackSection.vue'
import ExperienciaSection from '@/components/ExperienciaSection.vue'
import MentoriaSection from '@/components/MentoriaSection.vue'
</script>
