<template>
  <div class="relative inline-block text-left">
    <button
      type="button"
      class="inline-flex justify-center font-mitr-light text-[1rem] text-gray"
      @click="toggleDropdown"
    >
      {{ language }}
      <AppSvg
        v-if="isDropdownOpen"
        name="/assets/svg/language-switcher/down.svg"
        class="self-center pl-[0.5rem]"
      />
      <AppSvg
        v-if="!isDropdownOpen"
        name="/assets/svg/language-switcher/up.svg"
        class="self-center pl-[0.5rem]"
      />
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
import { ref, computed } from "vue";

const isDropdownOpen = ref<boolean>(false);
const selectedLanguage = ref<string>("EN");
const languages = ref<string[]>(["EN", "TH"]);

const toggleDropdown = (): void => {
  isDropdownOpen.value = !isDropdownOpen.value;
};

const toggleLanguage = (lang: string): void => {
  selectedLanguage.value = lang;
  isDropdownOpen.value = !isDropdownOpen.value;
};

const language = computed(() => selectedLanguage.value);
</script>
