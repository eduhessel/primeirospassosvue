<template> <!--HTML-->
    <h1>Meu nome é: {{ nome }}</h1> <!--Importando dados do script "nome"-->
</template>

<script> /* Javascript */
    export default {
        name: 'LifeCycle', /* Nome do script */
        data() { /* Dados */
            return { /* Retornará */
                nome: 'Ainda não sei' /* Dado que irá retornar no script "nome" */
            }
        },
        created() { /* Após ser criado os dados alterar dados em 1 segundo (pode ser usado como loading)*/
            setTimeout(() => {
                this.nome = 'Matheus' /* Dado que irá retornar */
            }, 1000); /* Tempo em mseg */
        },
        mounted() { /* Mostrando dados alterar dados em 2 segundos */
            setTimeout(() => {
                this.nome = 'Pedro' /* Dado que irá retornar */
            }, 2000); /* Tempo em mseg */
        }
    }
</script>