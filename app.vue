<script setup>
useSeoMeta({
  title: 'Blog | Denilson De La Rosa',
  description: 'El blog personal de un estudiante en sistemas computacionales'
})
</script>

<template>
  <div class="font-mono">
    <CustomNav />
    <NuxtPage class="h-1/3"/>
    <Fotter/>
  </div>
</template>

<style>
body {
  background-color: #F9F4EC;
}
</style>
