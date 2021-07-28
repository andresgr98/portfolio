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
  position: relative;
  font-size: 5rem;
}
.main-navbar-item {
  font-family: "Poppins", sans-serif;
}
#main-logo::before {
  transform: scaleX(0);
  transform-origin: bottom right;
}

#main-logo:hover::before {
  transform: scaleX(1);
  transform-origin: bottom left;
}

#main-logo::before {
  content: " ";
  display: block;
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  inset: 0 0 0 0;
  background: hsl(200 100% 80%);
  z-index: -1;
  transition: transform 0.3s ease;
}

html {
  block-size: 100%;
  inline-size: 100%;
}

body {
  min-block-size: 100%;
  min-inline-size: 100%;
  margin: 0;
  box-sizing: border-box;
  display: grid;
  place-content: center;
}

@media (orientation: landscape) {
  body {
    grid-auto-flow: column;
  }
}
</style>

