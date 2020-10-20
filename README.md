# coding

## configurar projeto
```
yarn install
```

### servidor para desenvolvimento
```
yarn serve
```

### compila e minifica para a produção
```
yarn build
```

### arruma os arquivos
```
yarn lint
```

### configuração personalizada 
veja [Configuration Reference](https://cli.vuejs.org/config/).


// para atualizar depois 

### use componentes com nomes compostos
	|- BaseCard
	|- ListItem


### o componente data deve ser uma funcão que retorna um objeto
	 data: function () {
    	  return {
           foo: 'bar'
          }
         }


### as propriedades devem ser o mais detalhado possivel 
	props: {
 	 status: String
	}

	ou

	props: {
	  status: {
	    type: String,
	    required: true
	  }
	}	


### para o v-for são necessárias keys
	<ul>
	  <li
	    v-for="todo in todos"
	    :key="todo.id"
	  >
	    {{ todo.text }}
	  </li>
	</ul>


### não use v-if e v-for no mesmo elemento
	<ul v-if="shouldShowUsers">
	  <li
	    v-for="user in users"
	    :key="user.id"
	  >
	    {{ user.name }}
	  </li>
	</ul>


### use scopo local para estilos, exceto no App.vue
	<template>
	  <button class="button button-close">X</button>
	</template>

	<!-- Usando o atributo `scoped` -->
	<style scoped>
	.button {
	  border: none;
	  border-radius: 2px;
	}

	.button-close {
	  background-color: red;
	}
	</style>


### use PascalCase
	|- MyComponent.vue


### componentes que terão apenas uma instância deverão começar como o prefixo The
	components/
	|- TheHeading.vue
	|- TheSidebar.vue


### componentes de uso geral deverão começar com o nome Base
	components/
	|- BaseButton.vue
	|- BaseTable.vue
	|- BaseIcon.vue


### componentes filhos devem conter o nome do componente pai como prefixo 
	components/
	|- SearchSidebar.vue
	|- NavigationForSearchSidebar.vue


### componentes devem ser chamados com kebab-case
	<my-component></my-component>


### para elementos de multiplos atributos deve sempre pular linhas
	<my-component
	  foo="a"
	  bar="b"
	  baz="c"
	/>

### use : para v-bind, @ para v-on e # para v-slot
	<input
	  :value="newTodoText"
	  :placeholder="newTodoInstructions"
	>

	<input
	  @input="onInput"
	  @focus="onFocus"
	>


### ordem de prioridade: template, script, style

### ao utilizar style scoped, sempre use classes

### props down, events up
