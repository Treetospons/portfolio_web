<template>
  <p class="font-mitr-light text-[1rem] text-gray ml-[2rem] hover:font-mitr hover:text-white">
    <span class="text-primary">#</span>{{ menu }}
  </p>
</template>

<script lang="ts" setup>
const { menu } = defineProps({
  menu: { type: String, required: true },
});
</script>
