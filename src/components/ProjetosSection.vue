<template>
  <section id="projetos" class="scroll-mt-20 px-6 py-24 md:px-16">
    <div class="mx-auto max-w-6xl">
      <div class="mb-12 max-w-2xl">
        <p class="mb-3 text-sm font-semibold uppercase tracking-widest text-secondary">
          Da interface à infraestrutura
        </p>
        <h2 class="mb-4 text-3xl font-bold text-ice md:text-4xl">Produtos Full-stack</h2>
        <p class="leading-relaxed text-gray-custom">
          Projetos em que participei de todo o ciclo: entendimento do problema, experiência
          do usuário, front-end, API, banco de dados e entrega.
        </p>
      </div>

      <div class="grid gap-6 lg:grid-cols-2">
        <article
          v-for="project in projects"
          :key="project.name"
          class="group flex flex-col rounded-xl border border-zinc-700 bg-white/[0.02] p-6 transition-all duration-300 hover:-translate-y-1 hover:border-secondary md:p-8"
        >
          <div class="mb-6 flex items-start justify-between gap-4">
            <div>
              <p class="mb-2 text-xs font-semibold uppercase tracking-widest text-secondary">
                {{ project.type }}
              </p>
              <h3 class="text-2xl font-semibold text-ice">{{ project.name }}</h3>
            </div>
            <span class="shrink-0 rounded-full border border-zinc-700 px-3 py-1 text-xs text-gray-custom">
              {{ project.status }}
            </span>
          </div>

          <p class="mb-6 text-sm leading-relaxed text-gray-custom">
            {{ project.description }}
          </p>

          <ul class="mb-6 space-y-2 text-sm text-gray-custom">
            <li v-for="highlight in project.highlights" :key="highlight" class="flex gap-2">
              <span class="text-secondary" aria-hidden="true">✓</span>
              <span>{{ highlight }}</span>
            </li>
          </ul>

          <div class="mt-auto">
            <div class="mb-6 flex flex-wrap gap-2">
              <span
                v-for="technology in project.technologies"
                :key="technology"
                class="rounded bg-blue-custom/20 px-2.5 py-1 text-xs text-blue-300"
              >
                {{ technology }}
              </span>
            </div>

            <a
              v-if="project.url"
              :href="project.url"
              target="_blank"
              rel="noopener noreferrer"
              class="inline-flex items-center gap-2 text-sm font-semibold text-secondary hover:underline"
            >
              Conhecer o projeto <span aria-hidden="true">→</span>
            </a>
            <span v-else class="text-sm text-zinc-400">Case em preparação</span>
          </div>
        </article>
      </div>
    </div>
  </section>
</template>

<script setup lang="ts">
interface Project {
  name: string
  type: string
  status: string
  description: string
  highlights: string[]
  technologies: string[]
  url?: string
}

const projects: Project[] = [
  {
    name: 'Gym Tracker',
    type: 'Produto autoral · Full-stack',
    status: 'Em desenvolvimento',
    description:
      'Plataforma para professores criarem planos de treino e acompanharem seus alunos, enquanto os alunos acessam e organizam sua rotina de exercícios.',
    highlights: [
      'Perfis distintos para professor e aluno com associação por código de convite.',
      'Criação de planos, fichas e exercícios com organização visual.',
      'API autenticada, modelagem relacional e controle de acesso por perfil.',
    ],
    technologies: ['Vue 3', 'TypeScript', 'Pinia', 'NestJS', 'Prisma', 'PostgreSQL', 'JWT'],
  },
  {
    name: 'Studio Leila Porto',
    type: 'Sistema em produção · Full-stack',
    status: 'Em produção',
    description:
      'Sistema de gestão para um estúdio de estética, criado a partir das necessidades reais do negócio para organizar procedimentos, solicitações e atendimento.',
    highlights: [
      'Levantamento de requisitos e definição dos principais fluxos do produto.',
      'Interface responsiva para operação e acompanhamento dos atendimentos.',
      'Desenvolvimento e publicação do front-end, API e banco de dados.',
    ],
    technologies: ['Angular', 'TypeScript', '.NET', 'C#', 'SQL Server'],
    url: 'https://studioleilaporto.com/login',
  },
  {
    name: 'Casa Musical',
    type: 'Projeto para cliente · Full-stack',
    status: 'Em produção',
    description:
      'Site institucional com sistema para captação, organização e acompanhamento de interessados em aulas experimentais.',
    highlights: [
      'Experiência institucional alinhada à identidade do negócio.',
      'Fluxo para registro e controle de aulas experimentais.',
      'Solução completa com interface, API e persistência de dados.',
    ],
    technologies: ['Angular', 'TypeScript', '.NET', 'C#'],
    url: 'https://www.casamusicalteresina.com/home',
  },
]
</script>
