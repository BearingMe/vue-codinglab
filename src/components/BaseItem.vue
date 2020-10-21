<template>
  <div class="col">
    <div
      class="row mt-4"
      data-aos="fade-in"
      data-aos-delay="200"
      data-aos-duration="800"
    >
      <!-- image  -->
      <div class="col-4 mb-3 px-0">
        <img :src="src" />
      </div>

      <!-- content  -->
      <div class="col">
        <div class="d-flex flex-column justify-content-between h-100">
          <div class="div">
            <h4 v-if="description" class="small text-white mt-2">
              {{ date }}
              <span v-if="tag">
                em <a class="text-info" href="#">{{ tag }}</a></span
              >
            </h4>
            <a :href="href"
              ><h3
                class="mt-2 mb-3"
                :class="description ? 'title-recents' : 'title-trends'"
              >
                {{ title }}
              </h3></a
            >
            <p v-if="description" class="description d-none d-md-inline">
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

          <ul v-if="description" class="social p-0 align-self-end">
            <li class="d-inline">
              <i class="fa fa-heart mr-2" aria-hidden="true"></i>
              <span class="social-number">{{
                Math.ceil(Math.random() * 20)
              }}</span>
            </li>
            <li class="d-inline ml-3">
              <i class="fa fa-comments mr-2" aria-hidden="true"></i>
              <span class="social-number">{{
                Math.ceil(Math.random() * 7)
              }}</span>
            </li>
            <li class="d-inline ml-3">
              <i class="far fa-bookmark" aria-hidden="true"></i>
            </li>
          </ul>
        </div>
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
    font-size: 1.5rem;
  }

  &-trends {
    font-size: 1rem;
  }
}

.description {
  font-weight: 300;
  font-size: 14px;
  color: rgba(223, 223, 223, 0.39);
}

.social {
  font-size: 14px;
}
</style>