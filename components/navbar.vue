<template>
  <b-navbar transparent centered spaced>
    <template #brand>
      <b-navbar-item id="main-logo" tag="router-link" :to="{ path: '/' }">
        AGR
      </b-navbar-item>
    </template>
    <template #start>
      <b-navbar-item
        tag="nuxt-link"
        :to="{ path: '/' }"
        class="main-navbar-item"
      >
        SOBRE MÍ
      </b-navbar-item>
      <b-navbar-item
        tag="nuxt-link"
        :to="{ path: '/projects' }"
        class="main-navbar-item"
        >PROYECTOS</b-navbar-item
      >
      <b-navbar-item
        tag="nuxt-link"
        :to="{ path: '/' }"
        class="main-navbar-item"
      >
        CONTACTO</b-navbar-item
      >
    </template>
  </b-navbar>
</template>


<script>
</script>


<style>
#main-logo {
  font-size: 3rem;
  font-family: "Lexend", sans-serif;
}
.main-navbar-item {
  font-family: "Poppins", sans-serif;
}
</style>

