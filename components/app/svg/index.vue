<template>
  <span v-if="icon" v-html="icon" />
</template>

<script lang="ts" setup>
const { name } = defineProps({
  name: String,
});

const temp = {
  ...import.meta.glob("/assets/svg/*.svg", {
    query: "?raw",
    import: "default",
  }),
  ...import.meta.glob("/assets/svg/*/*.svg", {
    query: "?raw",
    import: "default",
  }),
};

const icon = name && ((await temp[name]()) || name);
</script>
