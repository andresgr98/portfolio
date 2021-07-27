<template>
  <div>
    <navbar></navbar>
    <nuxt></nuxt>
  </div>
</template>

<script>
import Navbar from "~/components/navbar.vue";
export default {
  data() {
    return {
      Navbar,
    };
  },
};
</script>
