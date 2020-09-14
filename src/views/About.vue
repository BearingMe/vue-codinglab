<template>
  <div class="container">
    <div class="row mt-5">
      <!-- coluna principal  -->
      <div class="col-12">
        <h1 class="h3 text-uppercase font-italic font-weight-bold mb-4">Sobre o Projeto</h1>
        <p class="text-justify">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Nihil enim vitae veniam maiores voluptate rem obcaecati neque, incidunt commodi dolorem ducimus fugit! Enim quidem fuga dolor aspernatur consectetur corrupti quas.
          <br />Hic tenetur veniam exercitationem, numquam blanditiis sunt quam corporis dolores, impedit cum nulla repellendus eveniet magni recusandae? Odio itaque tempora saepe assumenda.
        </p>
      </div>
    </div>

    <div class="row mt-5">
      <!-- membro  -->
      <about-member
        picture="https://cdn.icon-icons.com/icons2/1736/PNG/512/4043272-avatar-lazybones-sloth-sluggard_113274.png"
        name="Smith"
        description="Conhecido por sua preguiça e completa falta de noção, é uma pessoa que pode ser descrito facilmente como retardado. É lembrado principalmente por falhas homéricas, como destruir uma dezena de distros Linux e estar quase sempre bêbado. Foi o maior responsável pelo design do site e consequentemente o atraso de mais de um ano na produção. Dizem que seu maior sonho é ser agricultor de cannabis."
        role="role-founder, role-developer, role-designer"
      />

      <about-member
        picture="https://cdn.icon-icons.com/icons2/483/PNG/512/art-palette_47204.png"
        name="Lorem"
        description="Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit provident incidunt voluptatem repellat itaque non quae explicabo debitis laudantium. Impedit sed praesentium quam minima ex! Incidunt a rem corporis esse!"
        role="role-developer"
      />

      <about-member
        picture="https://f0.pngfuel.com/png/980/886/male-portrait-avatar-png-clip-art.png"
        name="Ipsum"
        description="Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit provident incidunt voluptatem repellat itaque non quae explicabo debitis laudantium. Impedit sed praesentium quam minima ex! Incidunt a rem corporis esse!"
        role="role-contribuitor"
      />


    </div>
  </div>
</template>

<script>
import AboutMember from "../components/AboutMember";

export default {
  name: "About",

  head: {
    title: { inner: "Sobre Nós | Coding Community", separator: " " },
    mete: [
      {
        name: "description",
        content:
          "Alguns dos principais idealizadores e desenvolvedores da plataforma.",
      },
    ],
  },

  components: {
    AboutMember,
  },
};
</script>

<style>
</style>