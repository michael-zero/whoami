<template>
  <main class="bg-primary">
    <HeroSection />
    <hr class="border-zinc-800" aria-hidden="true" />
    <SobreSection />
    <hr class="border-zinc-800" aria-hidden="true" />
    <TechStackSection />
    <hr class="border-zinc-800" aria-hidden="true" />
    <ExperienciaSection />
    <hr class="border-zinc-800" aria-hidden="true" />
    <ProjetosSection />
    <hr class="border-zinc-800" aria-hidden="true" />
    <FormacaoSection />
    <!-- <hr class="border-zinc-800" />
    <ContatoSection /> -->
  </main>
  <AppFooter />
</template>

<script setup lang="ts">
import AppFooter from '@/components/AppFooter.vue'
import HeroSection from '@/components/HeroSection.vue'
import SobreSection from '@/components/SobreSection.vue'
import TechStackSection from '@/components/TechStackSection.vue'
import ExperienciaSection from '@/components/ExperienciaSection.vue'
import ProjetosSection from '@/components/ProjetosSection.vue'
import FormacaoSection from '@/components/FormacaoSection.vue'
// import ContatoSection from '@/components/ContatoSection.vue'
</script>
