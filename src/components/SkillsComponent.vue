<template>
    <div class="mt-6">
      <h2 class="text-2xl font-semibold mb-4">Habilidades</h2>
      <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-3">
        <div 
          v-for="skill in skills" 
          :key="skill" 
          class="bg-teal-600 text-white text-center py-2 px-2 rounded-lg shadow-md">
          {{ skill }}
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    props: {
      skills: Array,
    },
  };
  </script>
  