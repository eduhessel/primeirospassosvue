<template> <!--HTML-->
  <PrimeiroComponente /> <!--Componente-->
  <p> O dado do app é: {{ testando }}</p>
  <LifeCycle />
</template>

<script> /* Javascript */
  import PrimeiroComponente from './components/PrimeiroComponente.vue'
  import LifeCycle from './components/LifeCycle.vue'

  export default {
    name: 'App',
    components: {
      PrimeiroComponente,
      LifeCycle
    },
    data() {
      return{
        testando: "Teste"
      }
    }
  }
</script>