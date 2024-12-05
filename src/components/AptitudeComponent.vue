<template>
    <div class="mt-6">
      <h2 class="text-2xl font-semibold mb-4">Aptitudes</h2>
      <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-2 gap-3">
        <div 
          v-for="aptitude in aptitudes" 
          :key="aptitude" 
          class="bg-teal-600 text-white text-center py-2 px-2 rounded-lg shadow-md">
          {{ aptitude }}
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    props: {
      aptitudes: Array,
    },
  };
  </script>
  