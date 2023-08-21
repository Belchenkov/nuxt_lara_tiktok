<script setup>
  import { useRoute } from 'nuxt/app';

  const route = useRoute();
</script>

<template>
  <div
    id="topNav"
    class="fixed bg-white z-30 flex items-center w-full border-b h-[61px]"
  >
    <div
        class="flex items-center justify-between w-full px-6 mx-auto"
        :class="route.fullPath === '/' ? 'max-w-[1150px]' : ''"
    >
      <div :class="route.fullPath === '/' ? 'w-[80%]' : ''"></div>
    </div>
  </div>
</template>


<style scoped>

</style>
