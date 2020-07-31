<template>
  <nav class="navbar navbar-expand-sm navbar-dark bg-dark">
    <div class="container">
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
      <div class="collapse navbar-collapse" id="collapsibleNavId">
        <ul class="navbar-nav mx-auto">
          <!-- incio -->
          <li class="nav-item active">
            <a class="nav-link" href="#">
              Inicio
              <span class="sr-only">(current)</span>
            </a>
          </li>

          <!-- comunidade  -->
          <li class="nav-item">
            <a class="nav-link" href="#">Comunidade</a>
          </li>

          <!-- trabalhos  -->
          <li class="nav-item">
            <a class="nav-link" href="#">Trabalhos</a>
          </li>

          <!-- contato  -->
          <li class="nav-item">
            <a class="nav-link" href="#">Contato</a>
          </li>

          <!-- sobre  -->
          <li class="nav-item">
            <a class="nav-link" href="#">Sobre</a>
          </li>
        </ul>
      </div>

      <!-- social media  -->
      <div class="text-light">
        <!-- instagram  -->
        <a class="btn text-light" href="#" role="button">
          <i class="fa fa-lg fa-instagram" aria-hidden="true"></i>
        </a>

        <!-- facebook -->
        <a class="btn text-light" href="#" role="button">
          <i class="fa fa-lg fa-facebook" aria-hidden="true"></i>
        </a>

        <!-- twitter -->
        <a class="btn text-light" href="#" role="button">
          <i class="fa fa-lg fa-twitter" aria-hidden="true"></i>
        </a>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "TheNavbar",
};
</script>

