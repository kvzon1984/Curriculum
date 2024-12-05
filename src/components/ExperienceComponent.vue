<template>
  <div class="mt-6">
    <h2 class="text-2xl font-semibold">Experiencia</h2>

    <div class="flex flex-col gap-8 mt-4 ml-6" v-for="experience in experiences" :key="experience.title">
      <div class="flex items-start bg-gray-100 p-6">
        <div class="w-1/4">
          <p class="italic">{{ experience.location }}</p>
          <p>{{ experience.dates }}</p>
        </div>

        <div class="w-3/4 border-l-2 border-indigo-300 pl-4">
          <h3 class="text-xl font-bold">{{ experience.title }}</h3>
          <p class="italic font-semibold text-sky-400">{{ experience.company }}</p>
          
          <!-- Aquí se formatea la descripción de cada experiencia -->
          <div v-for="(paragraph, index) in formattedDescription(experience.description)" :key="index">
            <p class="text-gray-700 mb-2">{{ paragraph }}</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    experiences: Array,
  },
  methods: {
    // Método que formatea la descripción, separando por saltos de línea
    formattedDescription(description) {
      return description.split("\n").filter((paragraph) => paragraph.trim() !== "");
    },
  },
};
</script>
