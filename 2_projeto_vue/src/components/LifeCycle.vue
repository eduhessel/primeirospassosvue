<template> <!--HTML-->
    <h1>Meu nome é: {{ nome }}</h1>
</template>

<script>
    export default {
        name: 'LifeCycle',
        data() { /* Dados */
            return {
                nome: 'Ainda não sei'
            }
        },
        created() { /* Após ser criado os dados alterar dados em 1 segundo (pode ser usado como loading)*/
            setTimeout(() => {
                this.nome = 'Matheus'
            }, 1000);
        },
        mounted() { /* Mostrando dados alterar dados em 2 segundos */
            setTimeout(() => {
                this.nome = 'Pedro'
            }, 2000);
        }
    }
</script>