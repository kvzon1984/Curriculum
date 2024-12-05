<template>
    <div class="mt-6">
      <h2 class="text-2xl font-semibold">Idiomas</h2>
      <ul>
        <li class="py-6" v-for="language in languages" :key="language.name">
            <p class="font-semibold">{{ language.name }}</p>
            <p>{{ language.level }}</p>
        </li>
      </ul>
    </div>
  </template>
  
  <script>
  export default {
    props: {
      languages: Array,
    },
  };
  </script>
  