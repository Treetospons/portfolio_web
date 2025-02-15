<template>
  <div class="flex mt-[7.9375rem] justify-between">
    <div class="flex">
      <h1 class="font-mitr text-[2rem] text-white">
        <span class="text-primary">#</span>projects
      </h1>
      <span class="w-[31.9375rem] h-[0.0625rem] border border-primary self-center ml-[1rem]"/>
    </div>
    <div>
      <p class="font-mitr text-[1rem] text-white">{{ "View all ~~>" }}</p>
    </div>
  </div>
  <div class="grid grid-cols-3 gap-[1rem] mt-[3rem]">
    <div v-for="project in projects">
      <ProjectsCard
        :title="project.title"
        :tech-stacks="project.techStacks"
        :image="project.image"
        :description="project.description"
      />
    </div>
  </div>
</template>

<script lang="ts" setup>
import { ref } from "vue";

const projects = ref([
  {
    title: "ChertNodes",
    description: "Minecraft servers hosting",
    techStacks: ["HTML", "SCSS", "Python", "Flask"],
    image: "https://placehold.co/330x201.png",
  },
  {
    title: "ProtectX",
    description: "Discord anti-crash bot",
    techStacks: [
      "React",
      "Express",
      "Discord.js",
      "Node.js",
      "HTML",
      "SCSS",
      "Python",
      "Flask",
    ],
    image: "https://placehold.co/330x201.png",
  },
  {
    title: "Kahoot Answers Viewer",
    description: "Get answers to your kahoot quiz",
    techStacks: ["CSS", "Express", "Node.js"],
    image: "https://placehold.co/330x201.png",
  },
]);
</script>
