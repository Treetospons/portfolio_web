<template>
  <div class="w-[11.125rem] border border-gray">
    <h1 class="font-mitr text-white text-[1rem] p-[0.5rem]">{{ title }}</h1>
    <div class="border border-t-gray flex flex-wrap">
      <p v-for="item in techStacks" class="font-mitr-light text-gray text-[1rem] p-[0.5rem]">
        {{ item }}
      </p>
    </div>
  </div>
</template>

<script lang="ts" setup>
const { title, techStacks } = defineProps({
  title: String,
  techStacks: Array,
});
</script>
