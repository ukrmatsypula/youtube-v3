<template>
  <div class="relative">
    <img :src="`https://picsum.photos/seed/image${index}/720/404`" alt="" />
    <span
      class="absolute top-0 right-0 bg-black text-white rounded-sm m-1 p-1 opacity-0 bg-opacity-60 group-hover:opacity-100"
    >
      <BaseIcon name="clock" class="w-5 h-5" />
    </span>

    <span
      class="absolute top-8 right-0 bg-black text-white rounded-sm m-1 p-1 opacity-0 bg-opacity-60 group-hover:opacity-100"
    >
      <BaseIcon name="menuAlt3" class="w-5 h-5" /> </span
    ><span
      class="absolute bottom-0 right-0 bg-black text-white text-sm rounded-sm m-1 p-1 font-semibold opacity-100 group-hover:opacity-0 duration-500"
      >6:33</span
    >
  </div>
</template>

<script>
import BaseIcon from "./BaseIcon.vue";

export default {
  components: { BaseIcon },
  props: ["index"],
};
</script>

<style lang="scss" scoped></style>
