
  <template>
    <div class="mt-6">
      <h2 class="text-2xl font-semibold">Educación</h2>
      <div
        class="flex flex-col gap-8 mt-4 ml-6"
        v-for="education in educations"
        :key="education.title"
      >
        <div class="flex items-start bg-gray-100 p-6">
          <div class="w-1/4">
            <p class="italic">{{ education.location }}</p>
            <p>{{ education.dates }}</p>
          </div>
  
          <div class="w-3/4 border-l-2 border-indigo-300 pl-4">
            <h3 class="text-xl font-bold">{{ education.title }}</h3>
            <p class="italic font-semibold text-sky-400">{{ education.institution }}</p>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    props: {
      educations: Array,
    },
  };
  </script>
  