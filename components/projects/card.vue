<template>
  <div class="w-[20.625rem] border border-gray">
    <img :src="image" :alt="title" />
    <div class="border border-t-gray flex flex-wrap">
      <p v-for="item in techStacks" class="font-mitr-light text-gray text-[1rem] p-[0.5rem]">
        {{ item }}
      </p>
    </div>
    <div class="p-[1rem] border border-t-gray">
      <h1 class="font-mitr text-white text-[1.5rem]">{{ title }}</h1>
      <p class="font-mitr-light text-gray text-[1rem] py-[1rem]">{{ description }}</p>
      <Button title="Live <~>"/>
    </div>
  </div>
</template>

<script lang="ts" setup>
const { title, description, techStacks, image } = defineProps({
  title: String,
  description: String,
  techStacks: Array,
  image: String,
});
</script>
