<script setup>
const route = useRoute()
</script>

<template>
  <nav class="px-10 py-2 flex items-center justify-between border-2">
    <div>
      <nuxt-link to="/"><img class="h-16 w-auto" src="/img/logo.png" alt="Logo" /></nuxt-link>
    </div>
    <div class="flex justify-between items-center gap-4 text-lg font-semibold">
      <nuxt-link to="/" :class="route.path == '/' ? 'font-bold underline decoration-indigo-500 decoration-2 underline-offset-2' : ''"  class=" inline-block hover:font-bold">Blog</nuxt-link>
      <nuxt-link to="/about" :class="route.path == '/about' ? 'font-bold underline decoration-indigo-500 decoration-2 underline-offset-2' : ''" class="inline-block hover:font-bold">Sobre mí</nuxt-link>
    </div>
  </nav>
</template>
