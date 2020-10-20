<template>
  <div class="col">
    <div
      class="row mt-4"
      data-aos="fade-in"
      data-aos-delay="200"
      data-aos-duration="800"
    >
      <!-- image  -->
      <div class="col-3 mb-3 px-0">
        <img :src="src" />
      </div>

      <!-- content  -->
      <div class="col">
        <h4 v-if="description" class="small text-white">
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
          {{ readMore ? description : computedDescription }}
          <a
            class="read-more"
            v-if="descriptionOverflow"
            @click="readMore = !readMore"
          >
            {{ readMore ? "Ocultar" : "Ler mais" }}
          </a>
        </p>
      </div>
    </div>
  </div>
</template>

<script>
import AOS from "aos";
import "aos/dist/aos.css";

export default {
  name: "BaseItem",

  props: {
    src: String,
    date: String,
    tag: String,
    title: String,
    description: String,
    href: String,
  },

  data() {
    return {
      readMore: false,
    };
  },

  mounted() {
    AOS.init();
  },

  computed: {
    maxLettersShown() {
      return window.innerWidth / 7;
    },

    descriptionOverflow() {
      return this.description.length > this.maxLettersShown;
    },

    descriptionSliced() {
      return this.description.slice(0, this.maxLettersShown).trim() + "... ";
    },

    computedDescription() {
      if (this.descriptionOverflow) return this.descriptionSliced;
      return this.description;
    },
  },
};
</script>

<style lang="scss" scoped>
.title {
  font-weight: 500;

  &-recents {
    font-size: 1.25rem;
  }

  &-trends {
    font-size: 1rem;
  }
}

.description {
  font-weight: 300;
  font-size: 14px;
}
</style>