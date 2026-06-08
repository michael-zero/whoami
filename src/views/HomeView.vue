<template>
  <main class="bg-primary">

    <!-- HERO -->
    <section class="min-h-screen px-6 md:px-16 flex items-center">
      <div class="grid grid-cols-1 md:grid-cols-2 gap-12 w-full max-w-6xl mx-auto">

        <div class="flex flex-col justify-center gap-5">
          <p class="text-secondary text-sm font-semibold uppercase tracking-widest">
            Michael Lesley
          </p>

          <h1 class="text-5xl md:text-7xl font-bold text-ice leading-tight">
            Front-end<br />
            <span class="text-secondary">Developer</span>
          </h1>

          <p class="text-gray-custom text-base md:text-lg leading-relaxed max-w-md">
            Especialista em Angular, React e TypeScript. Crio interfaces modernas para
            finanças, saúde digital e produtos digitais.
          </p>

          <div class="flex gap-4 pt-2">
            <a href="https://linkedin.com/in/michael-lesley-9a1a02178" target="_blank"
               class="bg-blue-custom text-ice px-5 py-2.5 rounded text-sm font-medium hover:opacity-80 transition-opacity">
              LinkedIn
            </a>
            <a href="https://github.com" target="_blank"
               class="border border-gray-custom text-ice px-5 py-2.5 rounded text-sm font-medium hover:bg-ice hover:text-primary transition-colors">
              GitHub
            </a>
            <a href="mailto:mlmbufpi@gmail.com"
               class="text-gray-custom hover:text-secondary transition-colors text-sm flex items-center">
              Email →
            </a>
          </div>
        </div>

        <div class="flex flex-col justify-center items-center md:items-end">
          <div class="grid grid-cols-2 gap-3 w-full max-w-xs">
            <span class="bg-primary border border-secondary text-secondary text-center text-sm font-medium px-4 py-3 rounded">
              Angular
            </span>
            <span class="bg-primary border border-zinc-700 text-ice text-center text-sm font-medium px-4 py-3 rounded">
              React
            </span>
            <span class="bg-primary border border-zinc-700 text-ice text-center text-sm font-medium px-4 py-3 rounded">
              TypeScript
            </span>
            <span class="bg-primary border border-zinc-700 text-ice text-center text-sm font-medium px-4 py-3 rounded">
              RxJS
            </span>
            <span class="bg-primary border border-zinc-700 text-ice text-center text-sm font-medium px-4 py-3 rounded">
              Next.js
            </span>
            <span class="bg-primary border border-zinc-700 text-ice text-center text-sm font-medium px-4 py-3 rounded">
              Tailwind
            </span>
          </div>
        </div>

      </div>
    </section>

    <!-- SOBRE -->
    <section class="relative px-6 md:px-16 py-24 bg-[url('/fundo.jpg')] bg-cover bg-center bg-fixed">
      <div class="absolute inset-0 bg-primary/70" />

      <div class="relative z-10 max-w-6xl mx-auto">
        <h2 class="text-3xl md:text-4xl font-bold text-ice mb-12">
          Sobre
        </h2>

        <p class="text-gray-custom text-base md:text-lg leading-relaxed max-w-3xl">
          Desenvolvedor Front-end com experiência na criação, manutenção e evolução de
          aplicações web para os setores financeiro, saúde digital, serviços públicos e
          projetos freelancer. Atuação sólida com Angular, TypeScript, RxJS, React e Next.js,
          além de integrações com APIs, WebSocket, Firebase e Node.js.
        </p>
      </div>
    </section>

  </main>
  <AppFooter />
</template>

<script setup lang="ts">
import AppFooter from '@/components/AppFooter.vue'
</script>
