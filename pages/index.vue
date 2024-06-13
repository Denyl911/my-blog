<script setup>
const posts = ref([{
  id: 1,
  title: 'La Revolución Tecnológica de las Inteligencias Artificiales',
  desc: 'En la última década, hemos sido testigos de una verdadera revolución tecnológica protagonizada por las inteligencias artificiales (IA)...',
  date: '13 junio 2024',
  img: '/img/ai.jpg'
},
{
  id: 2,
  title: 'Comandos Esenciales de Linux que Debes Conocer',
  desc: 'Linux es un sistema operativo poderoso y flexible que se utiliza ampliamente en servidores y computadoras personales...',
  date: '12 junio 2024',
  img: '/img/term.jpg'
},
{
  id: 3,
  title: 'Explorando los Frameworks de Desarrollo Web',
  desc: 'Los frameworks de desarrollo web han revolucionado la forma en que se construyen y mantienen aplicaciones web...',
  date: '10 junio 2024',
  img: '/img/web2.jpg'
},
{
  id: 4,
  title: 'Diferencias entre SOAP y REST',
  desc: 'En el mundo de los servicios web, SOAP (Simple Object Access Protocol) y REST (Representational State Transfer)...',
  date: '9 junio 2024',
  img: '/img/code.jpg'
},
{
  id: 5,
  title: 'Cómo Crear tu Propio Sitio Web',
  desc: '¿Alguna vez has querido tener tu propio sitio web pero te has sentido abrumado por la complejidad...',
  date: '5 junio 2024',
  img: '/img/web1.jpg'
}])
</script>

<template>
  <div class="container text-center mx-auto">
    <h1 class="text-4xl font-bold my-5 underline-offset-2">Ultimos Post</h1>
    <div class="text-left grid grid-cols-1 md:grid-cols-3 gap-x-4 gap-y-6 p-6 h-[74vh] overflow-y-scroll overflow-x-visible">
      <Post class="mx-2 md:mx-0" v-for="p in posts" :id="p.id" :title="p.title" :desc="p.desc" :date="p.date" :key="p.id" :img="p.img"/>
    </div>
  </div>
</template>

