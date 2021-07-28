<template>
  <b-carousel-list v-model="test" :data="items" :items-to-show="2">
    <template #item="list">
      <div class="card">
        <div class="card-image">
          <figure class="image is-5by4">
            <nuxt-link to="/projects"><img :src="list.image" /></nuxt-link>
          </figure>
        </div>
        <div class="card-content">
          <div class="content">
            <p class="title is-6">{{ list.title }}</p>
            <p class="">{{ list.description }}</p>
            <b-field grouped>
              <p class="control" v-if="list.rating">
                <b-rate :value="list.rating" show-score disabled />
              </p>
            </b-field>
          </div>
        </div>
      </div>
    </template>
  </b-carousel-list>
</template>

<script>
export default {
  name: "carousel",
  data() {
    return {
      test: 0,
      items: [
        {
          title: "Bukmark",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quaerat harum cupiditate repellat neque totam ullam reiciendis exercitationem soluta, repellendus ipsum quas vitae sapiente ab nobis molestias in et deleniti pariatur?",
          image: "https://buefy.org/static/img/placeholder-1280x960.png",
        },
        {
          title: "Slide 2",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quaerat harum cupiditate repellat neque totam ullam reiciendis exercitationem soluta, repellendus ipsum quas vitae sapiente ab nobis molestias in et deleniti pariatur?",

          image: "https://buefy.org/static/img/placeholder-1280x960.png",
        },
        {
          title: "Slide 3",
          description:
            "Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quaerat harum cupiditate repellat neque totam ullam reiciendis exercitationem soluta, repellendus ipsum quas vitae sapiente ab nobis molestias in et deleniti pariatur?",

          image: "https://buefy.org/static/img/placeholder-1280x960.png",
        },
      ],
    };
  },
  methods: {
    info(value) {
      this.test = value;
    },
  },
};
</script>
