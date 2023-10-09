<template> <!--HTML-->
  <PrimeiroComponente /> <!--Componente-->
  <p> O dado do app é: {{ testando }}</p> <!--Importando dados do script "testando"-->
  <LifeCycle /> <!--Componente-->
  <Pessoa /> <!--Componente-->
</template>

<script> /* Javascript */
  import PrimeiroComponente from './components/PrimeiroComponente.vue' /* Importar script */
  import LifeCycle from './components/LifeCycle.vue' /* Importar script */
  import Pessoa from './components/Pessoa.vue' /* Importar script */

  export default {
    name: 'App', /* Nome do script */
    components: { /* Componentes da aplicação */
      PrimeiroComponente, /* Componente */
      LifeCycle, /* Componente */
      Pessoa, /* Componente */
    },
    data() { /* Dados */
      return{ /* Retornará */
        testando: "Teste" /* Dado que irá retornar no script "testando" */
      }
    }
  }
</script>