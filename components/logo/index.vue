<template>
  <div class="flex flex-row items-center">
    <AppSvg name="/assets/svg/logo/logo.svg"/>
    <h1 class="font-mitr-medium text-[1rem] text-white ml-[0.5rem]">{{ title }}</h1>
  </div>
</template>

<script lang="ts" setup>
const { title } = defineProps({
  title: String,
});
</script>
