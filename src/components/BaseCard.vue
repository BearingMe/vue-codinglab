<template>
  <div class="col-12 col-lg-6">
      <div class="row mt-4" data-aos="fade-up" data-aos-duration="800">
    <!-- content  -->
    <div class="col" data-aos="fade-up" data-aos-duration="500">
      <h4 class="small text-info">
           <a class="text-info" href="#">{{ tag }}</a>
      </h4>
      <a :href="href"
        ><h3 class="title">
          {{ title }}
        </h3></a
      >
    </div>

    <!-- image  -->
    <div class="col-4 mb-3" >
      <img :src="src" />
    </div>

  </div>
  </div>
</template>

<script>
import AOS from "aos";
import "aos/dist/aos.css";

export default {
  name: "BaseCard",

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
  font-weight: 400;
  font-size: 1rem;
}

</style>