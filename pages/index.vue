<template>
  <div class="container">
    <section class="section">
      <div class="columns">
        <div class="column is-one-quarter mr-3">
          <img
            src="@/static/img/IMG_0275.png"
            alt="Fotografia de Andrés Gómez"
            class="tile-image"
          />
        </div>
        <div class="column">
          <h3 class="title is-3">Sobre mí</h3>
          <p>
            Lorem ipsum dolor sit, amet consectetur adipisicing elit. Maxime
            sint fugit consequuntur officiis officia distinctio magni ad
            accusamus, ullam ratione tenetur modi, rerum voluptatibus sit
            laborum pariatur consectetur, natus reiciendis odit expedita hic
            dolor dolores corporis! Dolores nihil consequatur laborum minima
            facilis? Tempora necessitatibus reprehenderit quasi reiciendis dolor
            aspernatur velit nemo quas ad optio qui perspiciatis, laudantium
            expedita. Velit labore harum itaque facere magnam molestiae natus
            fugit, voluptates sint ad.
          </p>
        </div>
      </div>
    </section>
    <section class="section">
      <h3 class="title is-3">Proyectos recientes</h3>
      <carousel></carousel>
    </section>
  </div>
</template>

<script>
import Carousel from "~/components/carousel.vue";
export default {
  name: "index",

  components: { Carousel },
};
</script>
<style>
.tile-image {
  width: 100%;
}
</style>
