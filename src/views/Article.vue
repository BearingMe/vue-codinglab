<template>
  <div class="container">
    <div class="row mt-5">

			<!-- main article  -->
			<div class="col-12 main-article mb-4">
				<img src="https://img.ibxk.com.br/2020/09/11/11171200105462.jpg?w=600&h=600&mode=crop&scale=both" alt="">
				<h1> Podemos estar vivendo em uma rede neural? </h1>
			</div>

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
		BaseCard
	}
};
</script>

<style lang="scss" scoped>
.main-article {
	min-height: 450px;
	max-height: 500px;
	overflow: hidden;

}
</style>