<template>
  <div class="home">
    <div class="container">
      <div class="row mt-5">

        <!-- coluna principal  -->
        <div class="col-12 col-md-8">
          <h1 class="h3 text-uppercase font-italic font-weight-bold mb-4">Recentes</h1>

          
          <div class="btn-group w-100 mb-5">
            <button class="btn btn-info mr-2">Python</button>
            <button class="btn btn-info mr-2">JavaScript</button>
            <button class="btn btn-info mr-2">PHP</button>
            <button class="btn btn-info mr-2">C++</button>
          </div>

          <!-- itens  -->
          <home-item 
            src="https://img.ibxk.com.br/2020/09/11/11171200105462.jpg?w=600&h=600&mode=crop&scale=both"
            date="13/09/2020" 
            tag="Curiosidades"
            title="Podemos estar vivendo em uma rede neural?" 
            description="“Discutimos a possibilidade de que todo o universo em seu nível mais fundamental seja uma rede neural.” Essa frase está no parágrafo que apresenta o trabalho do físico Vitaly Vanchurin..."
            href="https://www.tecmundo.com.br/ciencia/177683-podemos-vivendo-rede-neural.htm"
          />

          <home-item 
            src="https://img.ibxk.com.br/2020/09/10/10145959025194.jpg?w=600&h=600&mode=crop&scale=both"
            date="12/09/2020" 
            tag="Segurança"
            title="350 empresas brasileiras já vazaram dados de usuários na internet em 2020" 
            description="Em meio à pandemia do novo coronavírus, as empresas se viram forçadas a migrar para o modelo de home office, e seus profissionais, que antes trabalhavam por trás de toda a camada de segurança do escritório, como firewall e antivírus, agora estão trabalhando direto de casa, com um nível de segurança inferior ao ambiente corporativo... "
            href="https://www.tecmundo.com.br/seguranca/177604-350-empresas-brasileiras-vazaram-dados-usuarios-internet-2020.htm"
          />

          <home-item 
            src="https://img.ibxk.com.br/2020/09/10/10200038085020.jpg?w=600&h=600&mode=crop&scale=both"
            date="12/09/2020" 
            tag="Técnologia"
            title="Ainda vale a pena comprar o Galaxy Note 10?"
            description="Após o lançamento do novo Galaxy Note20 da Samsung no começo de agosto, muito se tem falado sobre a relação de custo-benefício do aparelho que justifique o preço inicial de US$ 1 mil, cerca de R$ 5,6 mil na cotação atual..." 
            href="https://www.tecmundo.com.br/produto/177663-ainda-vale-pena-comprar-galaxy-note-10.htm"
          />

          <home-item 
            src="https://img.ibxk.com.br/2020/09/10/10160448178256.jpg?w=600&h=600&mode=crop&scale=both"
            date="12/09/2020" 
            tag="Entretenimento"
            title="As 10 melhores séries de ficção científica no Amazon Prime Video" 
            description="As séries de ficção científica estão cada vez mais em alta na TV e nos serviços de streaming. São diversas produções excelentes surgindo constantemente para a alegria dos fãs desse gênero."
            href="https://www.tecmundo.com.br/minha-serie/177651-10-melhores-series-ficcao-cientifica-amazon-prime-video.htm"
          />

          <home-item 
            src="https://img.ibxk.com.br/2020/09/11/11165554520451.jpg?w=600&h=600&mode=crop&scale=both"
            date="11/09/2020" 
            tag="entretenimento"
            title="Velozes & Furiosos 9: filme terá sequência no espaço" 
            description="A franquia Velozes & Furiosos costuma apresentar as sequências de ação mais frenéticas que o cinema tem visto nos últimos anos. E agora, isso deve ganhar um novo patamar."
            href="https://www.tecmundo.com.br/cultura-geek/177684-velozes-furiosos-9-filme-tera-sequencia-espaco.htm"
          />

        </div>

        
        <!-- coluna secundária  -->
        <div class="d-none d-md-block col-md">

        <!-- tendencias  -->
          <h2 class="h3 text-uppercase font-italic font-weight-bold">Tendências</h2>

          <home-item 
            src="https://img.ibxk.com.br/2020/09/10/10155812472245.jpg?w=420&h=420&mode=crop&scale=both"
            date="12/09/2020" 
            title="NASA une dados de diversos telescópios em imagens deslumbrantes" 
            href="https://www.tecmundo.com.br/ciencia/177630-nasa-une-dados-diversos-telescopios-imagens-deslumbrantes.htm"
          />

          <home-item 
            src="https://img.ibxk.com.br/2020/09/10/10151244780203.jpg?w=420&h=420&mode=crop&scale=both"
            date="11/09/2020" 
            title="LGPD: esclarecendo os papéis de controlador e operador" 
            href="https://www.tecmundo.com.br/seguranca/177606-lgpd-esclarecendo-papeis-controlador-operador.htm"
          />

          <home-item 
            src="https://img.ibxk.com.br/2020/09/11/11143605871366.jpg?w=420&h=420&mode=crop&scale=both"
            date="11/09/2020" 
            title="O Diabo de Cada Dia: confira as primeiras reações ao filme" 
            href="https://www.tecmundo.com.br/cultura-geek/177672-diabo-cada-dia-primeiras-reacoes-filme-netflix.htm"
          />

          <home-item 
            src="https://img.ibxk.com.br/2020/09/11/11173508068478.jpg?w=420&h=420&mode=crop&scale=both"
            date="09/09/2020" 
            title="China está construindo espaçoporto flutuante para lançar foguetes"
            href="https://www.tecmundo.com.br/ciencia/177682-china-construindo-espacoporto-flutuante-lancar-foguetes.htm" 
          />

        </div>
      </div>
    </div>
  </div>
</template>

<script>
import HomeItem from "@/components/HomeItem";

export default {
  name: "Home",

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
    HomeItem
  }
};
</script>

<style scoped>
.btn-group {
 max-width: 100%;
 overflow-x: auto;
}
</style>