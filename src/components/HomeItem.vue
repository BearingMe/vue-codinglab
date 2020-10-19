<template>
  <div class="row mt-4" data-aos="fade-in" data-aos-delay="200" data-aos-duration="800">
    <!-- image  -->
    <div class="col-4 mb-3" >
      <img :src="src" />
    </div>

    <!-- content  -->
    <div class="col" >
      <h4 class="small text-white">
        {{ date }}
        <span v-if="tag">
          em <a class="text-info" href="#">{{ tag }}</a></span
        >
      </h4>
      <a :href="href"
        ><h3 :class="description ? 'title-recents' : 'title-trends'">
          {{ title }}
        </h3></a
      >
      <p v-if="description" class="text-justify description d-none d-md-inline">
        {{ description }} <a class="text-white" :href="href">Ler Mais</a>
      </p>
    </div>
  </div>
</template>

<script>
import AOS from "aos";
import "aos/dist/aos.css";

export default {
  name: "HomeItem",

  props: {
    src: String,
    date: String,
    tag: String,
    title: String,
    description: String,
    href: String,
  },

  mounted() {
    AOS.init();
  },
};
</script>

<style lang="scss" scoped>
.title {
  font-weight: 500;

  &-recents {
    font-size: 1.5rem;
  }

  &-trends {
    font-size: 1rem;
  }
}

.description {
  font-weight: 300;
}
</style>