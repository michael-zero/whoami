<script setup lang="ts">
import { RouterView } from 'vue-router';
import AppHeader from '@/components/AppHeader.vue';
import ScrollTopButton from '@/components/ScrollTopButton.vue';

</script>

<template>
  <AppHeader />
  <RouterView/>
  <ScrollTopButton />
</template>

<style scoped></style>
