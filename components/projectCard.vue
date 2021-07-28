<template>
  <a class="box" :href="project.url">
    <img
      src="https://estaticos.muyinteresante.es/media/cache/1140x_thumb/uploads/images/gallery/609cf90e5bafe89d454761e7/cachorro-jack-russell_0.jpg"
      alt=""
    />
    <h4 class="title is-4">{{ project.name }}</h4>
    <p>{{ project.subtitle }}</p>
  </a>
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
