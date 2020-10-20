<template>
  <div class="home">
    <div class="container">
      <div class="row mt-5">
        <!-- coluna principal  -->
        <div class="col">
          <h1 class="h3 text-uppercase font-italic font-weight-bold mb-4">
            Recentes
          </h1>

          <div class="btn-group w-100 mb-5">
            <button class="btn btn-info mr-2">Python</button>
            <button class="btn btn-info mr-2">JavaScript</button>
            <button class="btn btn-info mr-2">PHP</button>
            <button class="btn btn-info mr-2">C++</button>
          </div>

          <!-- itens  -->
          <base-item
            src="https://img.ibxk.com.br/2020/09/11/11171200105462.jpg?w=600&h=600&mode=crop&scale=both"
            date="13/09/2020"
            tag="Curiosidades"
            title="Podemos estar vivendo em uma rede neural?"
            description="“Discutimos a possibilidade de que todo o universo em seu nível mais fundamental seja uma rede neural.” Essa frase está no parágrafo que apresenta o trabalho do físico Vitaly Vanchurin..."
            href="https://www.tecmundo.com.br/ciencia/177683-podemos-vivendo-rede-neural.htm"
          />

          <base-item
            src="https://img.ibxk.com.br/2020/09/10/10145959025194.jpg?w=600&h=600&mode=crop&scale=both"
            date="12/09/2020"
            tag="Segurança"
            title="350 empresas brasileiras já vazaram dados de usuários na internet em 2020"
            description="Em meio à pandemia do novo coronavírus, as empresas se viram forçadas a migrar para o modelo de base office, e seus profissionais, que antes trabalhavam por trás de toda a camada de segurança do escritório, como firewall e antivírus, agora estão trabalhando direto de casa, com um nível de segurança inferior ao ambiente corporativo... "
            href="https://www.tecmundo.com.br/seguranca/177604-350-empresas-brasileiras-vazaram-dados-usuarios-internet-2020.htm"
          />

          <base-item
            src="https://img.ibxk.com.br/2020/09/10/10200038085020.jpg?w=600&h=600&mode=crop&scale=both"
            date="12/09/2020"
            tag="Técnologia"
            title="Ainda vale a pena comprar o Galaxy Note 10?"
            description="Após o lançamento do novo Galaxy Note20 da Samsung no começo de agosto, muito se tem falado sobre a relação de custo-benefício do aparelho que justifique o preço inicial de US$ 1 mil, cerca de R$ 5,6 mil na cotação atual..."
            href="https://www.tecmundo.com.br/produto/177663-ainda-vale-pena-comprar-galaxy-note-10.htm"
          />

          <base-item
            src="https://img.ibxk.com.br/2020/09/10/10160448178256.jpg?w=600&h=600&mode=crop&scale=both"
            date="12/09/2020"
            tag="Entretenimento"
            title="As 10 melhores séries de ficção científica no Amazon Prime Video"
            description="As séries de ficção científica estão cada vez mais em alta na TV e nos serviços de streaming. São diversas produções excelentes surgindo constantemente para a alegria dos fãs desse gênero."
            href="https://www.tecmundo.com.br/minha-serie/177651-10-melhores-series-ficcao-cientifica-amazon-prime-video.htm"
          />

          <base-item
            src="https://img.ibxk.com.br/2020/09/11/11165554520451.jpg?w=600&h=600&mode=crop&scale=both"
            date="11/09/2020"
            tag="entretenimento"
            title="Velozes & Furiosos 9: filme terá sequência no espaço"
            description="A franquia Velozes & Furiosos costuma apresentar as sequências de ação mais frenéticas que o cinema tem visto nos últimos anos. E agora, isso deve ganhar um novo patamar."
            href="https://www.tecmundo.com.br/cultura-geek/177684-velozes-furiosos-9-filme-tera-sequencia-espaco.htm"
          />
        </div>

        <!-- coluna secundária  -->
        <div class="d-none d-lg-block col-4">
          <!-- tendencias  -->
          <h2 class="h3 text-uppercase font-italic font-weight-bold">
            Tendências
          </h2>

          <base-item
            src="https://img.ibxk.com.br/2020/09/10/10155812472245.jpg?w=420&h=420&mode=crop&scale=both"
            date="12/09/2020"
            title="NASA une dados de diversos telescópios em imagens deslumbrantes"
            href="https://www.tecmundo.com.br/ciencia/177630-nasa-une-dados-diversos-telescopios-imagens-deslumbrantes.htm"
          />

          <base-item
            src="https://img.ibxk.com.br/2020/09/10/10151244780203.jpg?w=420&h=420&mode=crop&scale=both"
            date="11/09/2020"
            title="LGPD: esclarecendo os papéis de controlador e operador"
            href="https://www.tecmundo.com.br/seguranca/177606-lgpd-esclarecendo-papeis-controlador-operador.htm"
          />

          <base-item
            src="https://img.ibxk.com.br/2020/09/11/11143605871366.jpg?w=420&h=420&mode=crop&scale=both"
            date="11/09/2020"
            title="O Diabo de Cada Dia: confira as primeiras reações ao filme"
            href="https://www.tecmundo.com.br/cultura-geek/177672-diabo-cada-dia-primeiras-reacoes-filme-netflix.htm"
          />

          <base-item
            src="https://img.ibxk.com.br/2020/09/11/11173508068478.jpg?w=420&h=420&mode=crop&scale=both"
            date="09/09/2020"
            title="China está construindo espaçoporto flutuante para lançar foguetes"
            href="https://www.tecmundo.com.br/ciencia/177682-china-construindo-espacoporto-flutuante-lancar-foguetes.htm"
          />
        </div>
      </div>
    </div>

    <div class="video-section my-5">
      <div class="container d-flex flex-column align-items-center text-center">
        <div class="video-logo">
          <img src="https://preview.colorlib.com/theme/thequest/img/logo-2.png" alt="" />
          <p>Melhores Shitposts</p>
        </div>
        <div class="video-popup-warp">
          <div class="video-image">
            <a
              href="https://www.youtube.com/watch?v=xzCEdSKMkdU"
              class="video-play"
              ><i class="fa fa-play"></i
            ></a>

          </div>
        </div>
      </div>
    </div>

    <contact class="my-5" />
  </div>
</template>

<script>
import BaseItem from "@/components/BaseItem";
import Contact from "./Contact";

export default {
  name: "home",

  head: {
    title: {
      inner: "Home | Coding Community",
      separator: " ",
    },
    meta: [
      {
        name: "description",
        content:
          "Aprenda a programar online com Python, Javascript, Java, PHP, C/C++, C# e várias outras linguagens.",
      },
      {
        name: "google-site-verification",
        content: "7N_vA5SF4MKiA8RLty31t3NFKlQ33pb_K12tIQHX-M0",
      },
    ],
  },

  components: {
    BaseItem,
    Contact,
  },
};
</script>

<style scoped>
.btn-group {
  max-width: 100%;
  overflow-x: auto;
}

.video-section {
    padding: 70px 0;
    background: #111111;
}

.video-logo {
    margin-bottom: 40px;
    max-width: 150px;
}

.video-popup-warp {
    position: relative;
}

.video-play i {
  display: block;
  border-radius: 50px;
  font-size: 100px;
  color: rgba(255, 255, 255, 0.582);
}

.video-image {
  background: url('https://i.pinimg.com/originals/20/cf/39/20cf39aadaae27be1f0da1e8303284e8.jpg');
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
  height: 50vh;
  width: 80vh;
  margin: 0;
  padding: 0;
  display: flex;
  justify-content: center;
  align-items: center;
}

</style>