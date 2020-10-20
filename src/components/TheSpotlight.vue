<template>
  <div
    class="spotlight-wrapper"
    :class="!(this.$route.name == 'Home') && 'halfscreen'"
  >
    <img
      class="spotlight"
      alt="Logo da linguagem Python"
      :src="require('@/assets/images/spotlight2.jpg')"
    />
  </div>
</template>

<script>
export default {
  name: "TheSpotlight",

  watch: {
    $route(to) {
      let div = document.querySelector(".spotlight-wrapper");
      let isHome = to.name == "Home";
      let maxHeight = window.innerHeight * (isHome ? 0.85 : 0.4);

      div.style.maxHeight = maxHeight + "px";
    },
  },
};
</script>

<style scoped>
.spotlight {
  min-height: 70vh;
  max-height: 85vh;
  width: 100%;
  object-fit: cover;
}

.spotlight-wrapper {
  overflow: hidden;
  transition: 500ms ease-in;
}

.halfscreen {
  filter: brightness(35%);
}
</style>