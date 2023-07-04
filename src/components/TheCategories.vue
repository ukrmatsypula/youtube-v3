<template>
  <section
    class="md:pl-24 xl:pl-64 pt-14 fixed bg-white w-full z-10 bg-opacity-95"
  >
    <div class="border-t border-b px-4 max-w-screen-2xl mx-auto">
      <div class="py-3 flex space-x-3 overflow-auto text-sm whitespace-nowrap">
        <CategoryItem
          v-for="(category, index) in categories"
          :key="index"
          :category="category"
          :isActive="category === 'All'"
        />
      </div>
    </div>
  </section>
</template>

<script>
import CategoryItem from "./CategoryItem.vue";
export default {
  components: { CategoryItem },
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
