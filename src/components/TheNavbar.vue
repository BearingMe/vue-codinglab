<template>
  <nav class="navbar navbar-expand-sm navbar-dark bg-dark py-sm-3 py-md-4">
    <div class="container bg-dark w-100">
      <!-- brand  -->
      <a class="navbar-brand" href="#">
        <img :src="require('@/assets/svg/brand.svg')" />
      </a>

      <!-- menu button  -->
      <button
        class="navbar-toggler border-0 d-lg-none"
        type="button"
        data-toggle="collapse"
        data-target="#collapsibleNavId"
        aria-controls="collapsibleNavId"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="navbar-toggler-icon"></span>
      </button>

      <!-- menu items  -->
      <div class="collapse navbar-collapse w-100" id="collapsibleNavId">
        <ul class="navbar-nav mx-auto">
          <!-- inicio -->
          <li class="nav-item">
            <router-link tag="a" class="nav-link" :to="{name: 'Home'}">Inicio</router-link>
            <span v-if="this.$route.name == ''" class="sr-only">(current)</span>
          </li>

          <!-- artigos  -->
          <li class="nav-item">
            <router-link tag="a" class="nav-link" :to="{name: 'Article'}">Artigos</router-link>
            <span v-if="this.$route.name == 'Article'" class="sr-only">(current)</span>
          </li>

          <!-- comunidade  -->
          <li class="nav-item">
            <router-link tag="a" class="nav-link" :to="{name: 'Community'}">Comunidade</router-link>
            <span v-if="this.$route.name == 'Community'" class="sr-only">(current)</span>
          </li>

          <!-- contato  -->
          <li class="nav-item">
            <router-link tag="a" class="nav-link" :to="{name: 'Contact'}">Contato</router-link>
            <span v-if="this.$route.name == 'Contact'" class="sr-only">(current)</span>
          </li>

          <!-- sobre  -->
          <li class="nav-item">
            <router-link tag="a" class="nav-link" :to="{name: 'About'}">Sobre</router-link>
            <span v-if="this.$route.name == 'About'" class="sr-only">(current)</span>
          </li>
        </ul>
      </div>

      <!-- social media  -->
      <div class="collapse navbar-collapse w-auto" id="collapsibleNavId">
        <ul class="navbar-nav ml-auto">
          <li class="nav-item d-inline-flex">
            <a class="nav-link mr-3 mr-sm-1" href="#">
              <i class="fab fa-instagram" aria-hidden="true"></i>
            </a>
            <a class="nav-link mr-3 mr-sm-1" href="#">
              <i class="fab fa-facebook" aria-hidden="true"></i>
            </a>
            <a class="nav-link mr-3 mr-sm-1" href="#">
              <i class="fab fa-twitter" aria-hidden="true"></i>
            </a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "TheNavbar",
};
</script>

<style lang="scss" scoped>
.router-link-exact-active {
  color: white !important;
}


</style>
