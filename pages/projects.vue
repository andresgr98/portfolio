<template>
  <div class="container">
    <section class="section">
      <h3 class="title is-3">Proyectos</h3>
      <div class="columns is-mobile">
        <div
          class="column is-one-quarter-desktop is-half-mobile"
          v-for="(item, index) in projects"
          :key="index"
        >
          <project-card :project="item"></project-card>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import ProjectCard from "~/components/projectCard.vue";
export default {
  name: "projects",
  components: {
    ProjectCard,
  },
  data() {
    return {
      projects: [
        {
          name: "Bukmark",
          subtitle: "Lorem ipsum dolor sit amet, consectetur",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quaerat harum cupiditate repellat neque totam ullam reiciendis exercitationem soluta, repellendus ipsum quas vitae sapiente ab nobis molestias in et deleniti pariatur?",
          image: "",
          url: "https://www.google.es",
        },
        {
          name: "Página personal",
          subtitle: "Lorem ipsum dolor sit amet, consectetur",
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
