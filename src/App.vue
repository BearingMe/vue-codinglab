<template>
  <div id="app">
    <header>
      <the-loginbar />
      <the-spotlight />
      <the-navbar />
    </header>

    <body>
      <router-view />
    </body>

    <footer>
      <the-footer />
    </footer>
  </div>
</template>

<script>
import TheLoginbar from "@/components/TheLoginbar.vue";
import TheNavbar from "@/components/TheNavbar.vue";
import TheFooter from "@/components/TheFooter.vue";
import TheSpotlight from "@/components/TheSpotlight.vue";

export default {
  components: {
    TheLoginbar,
    TheNavbar,
    TheFooter,
    TheSpotlight,
  }
};
</script>

<style lang="scss">
// todos os botões tem px-4
// a distância entre botões é de ml-3

body {
  background-color: #141414;
  color: #ffffff;
  min-height: 100vh;

  p {
    color: rgba($color: #ffffff, $alpha: 0.8);
  }
}

img {
  width: 100%;
  object-fit: cover;
}

a:hover {
  text-decoration: none;
}

.read-more {
  color: white !important;
  font-weight: bold;
  cursor: pointer;

  &:hover {
    color: darken($color: white, $amount: 10%) !important;
  }

  &:active {
    color: darken($color: white, $amount: 20) !important;
  }
}

.bg {
  &-transparent {
    background-color: transparent;
  }

  &-dark {
    background-color: #121212 !important;
  }
}

.text {
  &-light {
    filter: brightness(90%);
  }

  &-secondary {
    color: rgba(255, 255, 255, 0.658) !important;
  }
}

.navbar-brand * {
  max-height: 16px;
}

.btn {
  border-radius: 1px !important;
}

.btn-purple {
  background-color: #6f2b95;
  color: #ffffff;
}

.text-purple {
  color: #b01ba5;
}

.bg-dark-purple {
  background-color: #0c062e !important;
}

.bg-purple {
  background: linear-gradient(#421754, #331854);
  color: rgba(255, 255, 255, 0.822) !important;
}

.bg-transparent {
  background-color: transparent;
}

textarea,
input,
label,
button,
a {
  &:hover,
  &:focus,
  &:active,
  &:visited {
    outline: 0px !important;
    -webkit-appearance: none;
    box-shadow: none !important;
  }
}

.form-control {
  background-color: transparent;
  margin: 0 0 0.9rem;
  padding: 1.5rem 0;
  border: none;
  border-bottom: 1px rgba(255, 255, 255, 0.089) solid;
  border-radius: 0;

  &:focus {
    background-color: transparent;
    color: aliceblue;
    border-bottom-color: var(--info);
  }
}

input:-webkit-autofill,
input:-webkit-autofill:hover,
input:-webkit-autofill:focus,
textarea:-webkit-autofill,
textarea:-webkit-autofill:hover,
textarea:-webkit-autofill:focus,
select:-webkit-autofill,
select:-webkit-autofill:hover,
select:-webkit-autofill:focus {
  -webkit-text-fill-color: whitesmoke;
  transition: background-color 5000s ease-in-out 0s;
}
</style>
