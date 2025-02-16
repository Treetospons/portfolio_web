<template>
  <div class="fixed">
    <div class="w-[64rem] pt-[2rem] pb-[0.5rem] flex justify-between">
      <Logo title="Elias" />
      <div class="flex flex-row">
        <div v-for="item in menus">
          <LayoutHeaderMenu :menu="item.menu" />
        </div>
        <LanguageSwitcher class="pl-[2rem]" />
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup>
import { ref } from "vue";

const menus = ref([
  {
    menu: "home",
  },
  {
    menu: "works",
  },
  {
    menu: "about-me",
  },
  {
    menu: "contacts",
  },
]);
</script>
