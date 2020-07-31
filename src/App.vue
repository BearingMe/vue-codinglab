<template>
  <div id="app">
    <header>
      <the-loginbar />
      <img class="spotlight" :src="require('@/assets/images/spotlight.png')">
      <the-navbar />
    </header>


    <!-- <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>
    <router-view/> -->
  </div>
</template>

<script>
import TheLoginbar from '@/components/TheLoginbar.vue'
import TheNavbar from '@/components/TheNavbar.vue'

export default {
  components: {
    TheLoginbar,
    TheNavbar,
  }
}
</script>

<style lang="scss">
// todos os botões tem px-4
// a distância entre botões é de ml-3

.bg-transparent {
  background-color: transparent;
}

.navbar {
  height: 85px;
}

.bg-dark {
  background-color: #121212 !important;
}

.text-light {
  filter: brightness(90%);
}

.spotlight {
  min-height: 70vh;
  max-height: 85vh;
  width: 100%;
  object-fit: cover;
}

.navbar-brand * {
  max-height: 16px;
}

.btn {
  border-radius: 1px !important;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
