<template>
  <button
    type="button"
    class="inline-flex justify-center border border-primary px-[1rem] py-[0.5rem] font-mitr text-[1rem] text-white hover:bg-primary-hover"
  >
    {{ title }}
  </button>
</template>

<script lang="ts" setup>
const { title } = defineProps({
  title: String,
});
</script>
