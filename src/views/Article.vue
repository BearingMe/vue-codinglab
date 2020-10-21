<template>
  <div class="container">
    <!-- main article  -->
    <div class="row mt-5">
      <div class="col-12 main-article mb-4">
        <img
          src="https://img.ibxk.com.br/2020/09/11/11171200105462.jpg?w=600&h=600&mode=crop&scale=both"
          alt=""
        />
        <h1>Podemos estar vivendo em uma rede neural?</h1>
      </div>
    </div>

    <div class="row flex-column-reverse flex-lg-row">
      <div class="col">
        <div class="row">
          <base-card
            src="https://img.ibxk.com.br/2020/09/11/11171200105462.jpg?w=600&h=600&mode=crop&scale=both"
            date="13/09/2020"
            tag="Curiosidades"
            title="Podemos estar vivendo em uma rede neural?"
            href="https://www.tecmundo.com.br/ciencia/177683-podemos-vivendo-rede-neural.htm"
          />
          <base-card
            src="https://img.ibxk.com.br/2020/09/11/11171200105462.jpg?w=600&h=600&mode=crop&scale=both"
            date="13/09/2020"
            tag="Curiosidades"
            title="Podemos estar vivendo em uma rede neural?"
            href="https://www.tecmundo.com.br/ciencia/177683-podemos-vivendo-rede-neural.htm"
          />
          <base-card
            src="https://img.ibxk.com.br/2020/09/11/11171200105462.jpg?w=600&h=600&mode=crop&scale=both"
            date="13/09/2020"
            tag="Curiosidades"
            title="Podemos estar vivendo em uma rede neural?"
            href="https://www.tecmundo.com.br/ciencia/177683-podemos-vivendo-rede-neural.htm"
          />
          <base-card
            src="https://img.ibxk.com.br/2020/09/11/11171200105462.jpg?w=600&h=600&mode=crop&scale=both"
            date="13/09/2020"
            tag="Curiosidades"
            title="Podemos estar vivendo em uma rede neural?"
            href="https://www.tecmundo.com.br/ciencia/177683-podemos-vivendo-rede-neural.htm"
          />
        </div>
      </div>
      <div class="col-12 col-lg-3 mt-4">
        <div class="row">
					<!-- search -->
          <div class="card col-12 border-0 mb-4">
            <ul class="list-group">
              <li class="list-group-item header">
                Pesquisar <i class="fa fa-search float-right"></i>
              </li>
            </ul>
          </div>

					<!-- order -->
          <div class="card col-12 border-0 mb-4">
            <ul class="list-group">
              <li class="list-group-item header">
                Ordenar <i class="fa fa-sort float-right"></i>
              </li>
              <li class="list-group-item">Nome</li>
              <li class="list-group-item">Data</li>
              <li class="list-group-item">Curtidas</li>
            </ul>
          </div>

					<!-- filter -->
					<div class="card col-12 border-0 mb-4">
            <ul class="list-group">
              <li class="list-group-item header">
                Filtros <i class="fa fa-filter float-right"></i>
              </li>
              <li class="list-group-item">Linguagens</li>
              <li class="list-group-item">Frameworks</li>
              <li class="list-group-item">Autores</li>
              <li class="list-group-item">Tags</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import BaseCard from "@/components/BaseCard";

export default {
  name: "Article",

  head: {
    title: { inner: "Artigos | Coding Community", separator: " " },
    meta: [
      {
        name: "description",
        content:
          "Sessão contendo todo o conteúdo postado no site pelos administradores.",
      },
    ],
  },

  components: {
    BaseCard,
  },
};
</script>

<style lang="scss" scoped>
.main-article {
  min-height: 450px;
  max-height: 500px;
  overflow: hidden;
  position: relative;

  img {
    position: absolute;
    z-index: 0;
    filter: brightness(70%);
  }

  h1 {
    position: absolute;
    z-index: 1;
    bottom: 10%;
    text-align: center;
    font-size: 2rem;
    width: 100%;
    text-shadow: 5px 5px 10px black;
    color: #eee;
    font-weight: 500;
  }
}

.card,
.card * {
  border-radius: 0;
  background-color: transparent;
}

.list-group > .header {
  background-color: rgb(15, 15, 15);
}

.list-group-item {
  background-color: transparent;
}
</style>