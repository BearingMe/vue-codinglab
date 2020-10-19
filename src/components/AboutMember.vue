<template>
  <article class="container mb-5">
    <div class="row">
      <div class="col-auto pr-0">
        <figure class="rounded-circle bg-info">
          <img
            :src="picture"
            class="profile-pic rounded-circle"
            alt="Imagem de perfil"
          />
        </figure>
      </div>
      <div class="col">
        <div>
          <span class="name text-white">{{ name }}</span>
          <span
            v-for="(value, index) in roleArray"
            :key="index"
            class="role"
            :class="value"
          >
            {{ classes[value.trim()] }}
          </span>
        </div>
        <hr class="bg-info my-2" />

        <p class="d-inline">
          {{ readMore ? description : computedDescription }}
          <a
            class="read-more"
            v-if="descriptionOverflow"
            @click="readMore = !readMore"
          >
            {{ readMore ? "" : "Ler mais" }}
          </a>
        </p>
      </div>
    </div>
  </article>
</template>

<script>
export default {
  name: "AboutMember",

  props: {
    picture: String,
    name: String,
    description: String,
    details: Boolean,
    role: String,
  },

  data() {
    return {
      readMore: false,
      classes: {
        "role-developer": "Web Developer",
        "role-founder": "Membro Fundador",
        "role-designer": "UI/UX Designer",
        "role-contribuitor": "Contribuidor",
      },
    };
  },

  computed: {
    roleArray() {
      let roles = this.role.split(",");
      return roles.reverse();
    },

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
@import url("https://fonts.googleapis.com/css?family=Poppins&display=swap");

figure {
  padding: 3px;
}

.profile-pic {
  width: 85px;
  height: 85px;
}

.name {
  font-size: 16px;
  font-weight: 500;
}

.role {
  @media only screen and (max-width: 768px) {
    display: none;
  }

  position: relative;
  top: -5px;
  padding: 4px 10px;
  margin-left: 8px;
  font-size: 12px;
  border-radius: 6px;
  float: right;

  &-designer {
    background-color: rgb(1, 155, 152);
    box-shadow: 0 8px 16px 0 rgba(0, 184, 181, 0.4);
  }

  &-developer {
    background-color: #d14c8a;
    box-shadow: 0 8px 16px 0 rgba(231, 105, 150, 0.4);
  }

  &-founder {
    background-color: #6c5ce7;
    box-shadow: 0 5px 16px 0 rgba(128, 111, 253, 0.548);
  }

  &-contribuitor {
    background-color: #df6b44;
    box-shadow: 0 8px 16px 0 rgba(196, 105, 77, 0.4);
  }
}
</style>