<template>
  <div class="relative inline-block text-left">
    <button type="button" class="inline-flex justify-center" @click="toggleDropdown">
      {{ language }}
      <svg
        class="-mr-1 size-5 text-gray-400"
        viewBox="0 0 20 20"
        fill="currentColor"
        aria-hidden="true"
        data-slot="icon"
      >
        <path
          fill-rule="evenodd"
          d="M5.22 8.22a.75.75 0 0 1 1.06 0L10 11.94l3.72-3.72a.75.75 0 1 1 1.06 1.06l-4.25 4.25a.75.75 0 0 1-1.06 0L5.22 9.28a.75.75 0 0 1 0-1.06Z"
          clip-rule="evenodd"
        />
      </svg>
    </button>
    <div
      v-if="isDropdownOpen"
      class="absolute right-0 z-10 mt-2 border border-gray origin-top-right focus:outline-hidden"
    >
      <div v-for="language in languages">
        <a
          href="#"
          class="block px-[0.5rem] py-[0.5rem] text-gray"
          @click="toggleLanguage(language)"
          >{{ language }}</a
        >
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup>
import { ref } from "vue";
const isDropdownOpen = ref<boolean>(false);
const language = ref<string>("EN");
const languages = ref<string[]>(["EN", "TH"]);

const toggleDropdown = (): void => {
  isDropdownOpen.value = !isDropdownOpen.value;
};

const toggleLanguage = (lang: string): void => {
  language.value = lang;
  isDropdownOpen.value = !isDropdownOpen.value;
};
</script>
