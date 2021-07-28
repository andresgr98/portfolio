<template>
  <div class="box tile">
    <h4 class="title is-4">{{ project.name }}</h4>
    <p>{{ project.description }}</p>
  </div>
</template>

<script>
export default {
  name: "project-card",
  props: {
    project: Object,
  },
};
</script>

<style>
</style>
