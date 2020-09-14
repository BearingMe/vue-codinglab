<template>
  <div class="row mt-4">
    <div class="col-12 col-md-5 mb-3">
      <img
        :src="src"
      />
    </div>
    <div class="col-12 col-md-7">
      <h4 class="small text-white">
        {{date}}
        <span v-if="tag">
            em
            <a class="text-primary" href="#">{{tag}}</a>
        </span>
      </h4>
      <a :href="href"><h3 class="text-white" :class="description? 'h4': 'h6'">{{title}}</h3></a>
      <p v-if="description" class="text-secondary text-justify">
        {{description}} <a class="text-white" :href="href">Ler Mais</a>
      </p>
    </div>
  </div>
</template>

<script>
export default {
    name: 'HomeItem',

    props: {
        src: String, 
        date: String, 
        tag: String,
        title: String, 
        description: String,
        href: String
    }
};
</script>

<style>
</style>