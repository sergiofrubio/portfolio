<template>
  <nav class="navbar navbar-expand-lg navbar-light bg-light">
    <div class="container-fluid">
      <!-- <a class="navbar-brand" href="#">My Portfolio</a> -->
      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarNav"
        aria-controls="navbarNav"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav ms-auto">
          <li class="nav-item">
            <router-link class="nav-link" to="/">Inicio</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/about">Sobre mí</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/projects">Proyectos</router-link>
          </li>
          <!-- <li class="nav-item">
            <router-link class="nav-link" to="/contact">Contacto</router-link>
          </li> -->
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'Navbar',
}
</script>

<style scoped>
.navbar-brand {
  font-weight: bold;
}
</style>
