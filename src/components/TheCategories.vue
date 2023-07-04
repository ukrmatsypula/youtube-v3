<template>
  <section
    class="md:pl-24 xl:pl-64 pt-14 fixed bg-white w-full z-10 bg-opacity-95"
  >
    <div class="border-t border-b px-4 max-w-screen-2xl mx-auto">
      <div class="py-3 flex space-x-3 overflow-auto text-sm whitespace-nowrap">
        <a
          v-for="(categoty, index) in categories"
          :key="index"
          href="#"
          class="px-3 py-1 transition bg-gray-600 border border-gray-700 rounded-full hover:bg-gray-500 text-white"
          >{{ categoty }}</a
        >
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data: () => ({
    categories: [
      "All",
      "Trucks",
      "Tools",
      "Machines",
      "Engines",
      "Show",
      "Ships",
      "Roads",
      "Tanks",
      "Buildings",
      "Mars",
      "Woodworking",
      "Football",
      "TV Shows",
      "Songs",
      "Tractors",
      "Woodworking",
      "Woodworking",
    ],
  }),
};
</script>
