<template>
  <nav class="loginbar navbar navbar-expand-sm navbar-dark bg-tranparent py-3">
    <div class="container">
      <div class="button-group ml-auto">
        <a class="text-light" type="submit">Registrar</a>
        <button class="btn btn-outline-light px-4 py-1 py-md-2 ml-3" type="submit">Login</button>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "TheLoginbar",
};
</script>

<style lang="scss">
.loginbar {
  position: absolute;
  width: 100%;
  top: 0;
}
</style>

