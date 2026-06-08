<template>
  <section class="px-6 md:px-16 py-24">
    <div class="max-w-6xl mx-auto">
      <h2 class="text-3xl md:text-4xl font-bold text-ice mb-12">
        Contato
      </h2>

      <form
        action="https://api.web3forms.com/submit"
        method="POST"
        class="max-w-lg space-y-5"
      >
        <input type="hidden" name="access_key" value="SUA_CHAVE_AQUI" />
        <input type="hidden" name="from_name" value="Formulário Portfólio" />
        <input type="hidden" name="subject" value="Novo contato do portfólio" />

        <div>
          <label for="nome" class="block text-sm text-gray-custom mb-1">Nome</label>
          <input
            id="nome"
            name="nome"
            type="text"
            required
            class="w-full bg-primary border border-zinc-700 rounded px-4 py-2.5 text-ice placeholder-zinc-500 focus:outline-none focus:border-secondary transition-colors"
            placeholder="Seu nome"
          />
        </div>

        <div>
          <label for="email" class="block text-sm text-gray-custom mb-1">Email</label>
          <input
            id="email"
            name="email"
            type="email"
            required
            class="w-full bg-primary border border-zinc-700 rounded px-4 py-2.5 text-ice placeholder-zinc-500 focus:outline-none focus:border-secondary transition-colors"
            placeholder="seu@email.com"
          />
        </div>

        <div>
          <label for="mensagem" class="block text-sm text-gray-custom mb-1">Mensagem</label>
          <textarea
            id="mensagem"
            name="mensagem"
            rows="5"
            required
            class="w-full bg-primary border border-zinc-700 rounded px-4 py-2.5 text-ice placeholder-zinc-500 focus:outline-none focus:border-secondary transition-colors resize-none"
            placeholder="Sua mensagem..."
          ></textarea>
        </div>

        <button
          type="submit"
          class="bg-blue-custom text-ice px-6 py-2.5 rounded text-sm font-medium hover:opacity-80 transition-opacity"
        >
          Enviar →
        </button>
      </form>
    </div>
  </section>
</template>

<script setup lang="ts">
</script>
