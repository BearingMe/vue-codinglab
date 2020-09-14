<template>
  <div class="container">
    <div class="row mt-5">
       <!-- coluna principal  -->
        <div class="col">
           <p class="text-center text-md-left text-white text-center mb-4">Envie uma mensagem</p>
           <form>
              <!-- nome  -->
              <input
                type="text"
                class="form-control"
                placeholder="Seu nome"
                required
                maxlength="100"
              />

              <!-- email -->
              <input
                type="email"
                class="form-control"
                placeholder="Seu email"
                required
                maxlength="100"
              />

              <!-- assunto  -->
              <input type="text" class="form-control" placeholder="Assunto" maxlength="100" />

              <!-- mensagem  -->
              <textarea
                class="form-control"
                rows="4"
                placeholder="Como podemos ajudar?"
                required
                maxlength="1000"
              ></textarea>

              <button class="btn btn-info btn-block text-shadow my-3">Enviar</button>
            </form>

         
        </div>

        
        <!-- coluna secundária  -->
        <div class="col-md-auto text-center text-md-left">

        <!-- tendencias  -->
           <p class=" text-white text-center mb-4">Informações de Contato</p>
              <!-- endereço -->
              <div class="mb-4">
                <p class="h6 text-info mb-2">Onde nos encontrar?</p>
                <p class="text-secondary mb-1">https://www.google.com.br</p>
                <p class="text-secondary mb-1">https://br.bing.com</p>
                <p class="text-secondary mb-1">https://br.yahoo.com</p>
              </div>

              <!-- email -->
              <div class="mb-4">
                <p class="h6 text-info mb-2">Nossos Emails</p>
                <p class="text-secondary mb-1">deos@xvi.com</p>
                <p class="text-secondary mb-1">ter@hams.com</p>
                <p class="text-secondary mb-1">tube@red.com</p>
              </div>

              <!-- email -->
              <div class="mb-4">
                <p class="h6 text-info mb-2">Nossos Números</p>
                <p class="text-secondary mb-1">+55 11 40028922</p>
                <p class="text-secondary mb-1">+55 34 999784767</p>
              </div>


              </div>
            </div>

        </div>
</template>

<script>
export default {
  name: "Contact",

  head: {
    title: { inner: "Contato | Coding Community", separator: " " },
    mete: [
      {
        name: "description",
        content: "Algum problema ou sugestão? Fale conosco.",
      },
    ],
  },
};
</script>

<style>
</style>