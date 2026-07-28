<template>
  <section id="inicio" class="relative overflow-hidden min-h-screen px-6 pt-24 md:px-16 flex items-center">
    <div class="grid grid-cols-1 md:grid-cols-2 gap-12 w-full max-w-6xl mx-auto">

      <div class="flex flex-col justify-center gap-5">
        <p class="text-secondary text-sm font-semibold uppercase tracking-widest opacity-0 translate-y-4 animate-fade-in [animation-delay:0ms]">
          Michael Lesley
        </p>

        <h1 class="text-5xl md:text-7xl font-bold text-ice leading-tight opacity-0 translate-y-4 animate-fade-in [animation-delay:200ms]">
          Front-end<br />
          <span class="text-secondary">Specialist</span>
        </h1>

        <p class="text-gray-custom text-base md:text-lg leading-relaxed max-w-md opacity-0 translate-y-4 animate-fade-in [animation-delay:400ms]">
          Desenvolvedor Front-end com experiência Full-stack. Construo produtos digitais
          completos para finanças, saúde, serviços públicos e negócios.
        </p>

        <div class="flex flex-wrap gap-3 pt-2">
          <a href="#projetos"
             class="bg-blue-custom text-ice px-4 py-2 rounded text-sm font-medium hover:opacity-80 transition-opacity">
            Ver projetos
          </a>
          <a href="https://github.com/michael-zero" target="_blank" rel="noopener noreferrer"
             class="border border-gray-custom text-ice px-4 py-2 rounded text-sm font-medium hover:bg-ice hover:text-primary transition-colors">
            GitHub
          </a>
          <a href="mailto:mlmbufpi@gmail.com"
             class="text-gray-custom hover:text-secondary transition-colors text-sm flex items-center">
            Vamos conversar →
          </a>
        </div>
      </div>

      <div class="flex flex-col justify-center items-center md:items-end">
        <div class="grid grid-cols-2 gap-3 w-full max-w-xs">
          <span class="bg-primary border border-secondary text-secondary text-sm font-medium px-4 py-3 rounded flex items-center justify-center gap-1.5">
            <img src="https://cdn.simpleicons.org/angular/ffffff" class="w-4 h-4" alt="" />Angular
          </span>
          <span class="bg-primary border border-zinc-700 text-ice text-sm font-medium px-4 py-3 rounded flex items-center justify-center gap-1.5">
            <img src="https://cdn.simpleicons.org/react/ffffff" class="w-4 h-4" alt="" />React
          </span>
          <span class="bg-primary border border-zinc-700 text-ice text-sm font-medium px-4 py-3 rounded flex items-center justify-center gap-1.5">
            <img src="https://cdn.simpleicons.org/typescript/ffffff" class="w-4 h-4" alt="" />TypeScript
          </span>
          <span class="bg-primary border border-zinc-700 text-ice text-sm font-medium px-4 py-3 rounded flex items-center justify-center gap-1.5">
            <img src="https://cdn.simpleicons.org/vuedotjs/ffffff" class="w-4 h-4" alt="" />Vue
          </span>
          <span class="bg-primary border border-zinc-700 text-ice text-sm font-medium px-4 py-3 rounded flex items-center justify-center gap-1.5">
            <img src="https://cdn.simpleicons.org/nodedotjs/ffffff" class="w-4 h-4" alt="" />Node.js
          </span>
          <span class="bg-primary border border-zinc-700 text-ice text-sm font-medium px-4 py-3 rounded flex items-center justify-center gap-1.5">
            <img src="https://cdn.simpleicons.org/dotnet/ffffff" class="w-4 h-4" alt="" />.NET
          </span>
        </div>
      </div>

    </div>
  </section>
</template>

<style scoped>
section::before {
  content: '';
  position: absolute;
  top: -50%;
  right: -20%;
  width: 700px;
  height: 700px;
  background: radial-gradient(circle, rgba(161,255,98,0.08) 0%, rgba(104,64,255,0.04) 50%, transparent 70%);
  pointer-events: none;
}

section::after {
  content: '';
  position: absolute;
  bottom: -30%;
  left: -10%;
  width: 500px;
  height: 500px;
  background: radial-gradient(circle, rgba(104,64,255,0.06) 0%, transparent 60%);
  pointer-events: none;
}

@keyframes fade-in {
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

.animate-fade-in {
  animation: fade-in 0.6s ease-out forwards;
}
</style>

<script setup lang="ts">
</script>
