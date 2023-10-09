<template> <!--HTML-->
  <PrimeiroComponente /> <!--Componente-->
  <p> O dado do app é: {{ testando }}</p>
</template>

<script> /* Javascript */
  import PrimeiroComponente from './components/PrimeiroComponente.vue'

  export default {
    name: 'App',
    components: {
      PrimeiroComponente
    },
    data() {
      return{
        testando: "Teste"
      }
    }
  }
</script>