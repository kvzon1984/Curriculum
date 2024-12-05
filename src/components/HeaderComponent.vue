<template>
    <header class="bg-teal-600 text-white p-8 rounded-lg">
      <div class="text-center">
        <h1 class="text-3xl font-bold">{{ header[0].name }}</h1>
        <p class="text-lg">{{ header[0].jobTitle }}</p>
        <p class="mt-2">{{ header[0].address }}</p>
        <p>{{ header[0].phone }} | {{ header[0].email }}</p>
        
        <!-- Ajuste del enlace -->
        <div class="my-4">
          <a
            href="header[0].linkedin"
            target="_blank"
            class="text-blue-200 hover:underline text-xl"
          >
            LinkedIn
          </a> 
          | 
          <a
            href="header[0].github"
            target="_blank"
            class="text-blue-200 hover:underline text-xl"
          >
            GitHub
          </a>
        </div>
      </div>
  
      <div v-for="(paragraph, index) in formattedDescription(header[0].objective)" :key="index">
            <p class="text-slate-200 mb-2 text-justify leading-relaxed px-8">{{ paragraph }}</p>
          </div>
    </header>
  </template>
  
  
  <script>
  export default {
    props: {
      header: Array,
    },
    methods: {
    formattedDescription(description) {
      return description.split("\n").filter((paragraph) => paragraph.trim() !== "");
    },
  },
  };
  </script>
  