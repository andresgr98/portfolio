<template>
  <div class="container">
    <h3 class="title is-3">Proyectos</h3>
    <div class="columns tile-ancestor">
      <div class="column" v-for="(item, index) in projects" :key="index">
        <project-card project="`${item}`"></project-card>
      </div>
    </div>
  </div>
</template>

<script>
import ProjectCard from "~/components/projectCard.vue";
export default {
  components: {
    ProjectCard,
  },
  data() {
    return {
      projects: [
        {
          name: "Bukmark",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quaerat harum cupiditate repellat neque totam ullam reiciendis exercitationem soluta, repellendus ipsum quas vitae sapiente ab nobis molestias in et deleniti pariatur?",
          image: "",
        },
        {
          name: "Página personal",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quaerat harum cupiditate repellat neque totam ullam reiciendis exercitationem soluta, repellendus ipsum quas vitae sapiente ab nobis molestias in et deleniti pariatur?",
          image: "",
        },
      ],
    };
  },
};
</script>

<style>
</style>
