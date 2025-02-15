<template>
  <div class="flex mt-[6.625rem] mb-[0.75rem] justify-between">
    <div class="flex">
      <h1 class="font-mitr text-[2rem] text-white">
        <span class="text-primary">#</span>skills
      </h1>
      <span class="w-[14.9375rem] h-[0.0625rem] border border-primary self-center ml-[1rem]"/>
    </div>
  </div>
  <div class="flex justify-between">
    <div class="ml-[2rem] self-center">
      <AppSvg name="/assets/svg/skills/logo.svg" />
    </div>
    <div class="grid grid-cols-3 gap-[1rem] mt-[3rem] self-center">
      <div v-for="skill in skills">
        <SkillsCard :title="skill.title" :tech-stacks="skill.techStacks" />
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup>
import { ref } from "vue";
const skills = ref([
  {
    title: "Languages",
    techStacks: ["TypeScript", "Lua", "Python", "JavaScript"],
  },
  {
    title: "Databases",
    techStacks: ["SQLite", "PostgreSQL", "Mongo"],
  },
  {
    title: "Tools",
    techStacks: [
      "VSCode",
      "Neovim",
      "Linux",
      "Figma",
      "XFCE",
      "Arch",
      "Git",
      "Font Awesome",
    ],
  },
  {
    title: "Other",
    techStacks: ["HTML", "CSS", "EJS", "SCSS", "REST", "Jinja"],
  },
  {
    title: "Frameworks",
    techStacks: ["React", "Vue", "Disnake", "Discord.js", "Flask", "Express.js"],
  },
]);
</script>
