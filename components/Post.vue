<script setup>
const props = defineProps(['id' ,'title', 'desc', 'date', 'img'])
</script>

<template>
    <nuxt-link :to="`/posts/${props.id}`" class="shadow p-4 rounded-md transition-transform duration-300 transform ease-in-out hover:scale-110 hover:z-10 bg-white">
        <img class="rounded" :src="props.img" alt="Post Banner" />
        <h3 class="font-semibold text-xl pt-2">{{ props.title }}</h3>
        <p class="py-1">
            {{ props.desc }}
        </p>
        <div class="flex items-center gap-3">
          <img src="/img/user.png" alt="User image" />
          <div>
            <h5 class="font-bold">Denilson De La Rosa</h5>
            <p>{{ props.date }}</p>
          </div>
        </div>
      </nuxt-link>
</template>