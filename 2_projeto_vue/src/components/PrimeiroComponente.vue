<template> <!--HTML-->
    <div>
        <h1>Olá Vue!</h1>
        <p>Meu nome é {{  nome }} e trabalho como {{ profissao }}</p> <!--Importando dados do script "profissao"-->
    </div>
</template>

<script> /* Javascript */
    export default{
        name: 'PrimeiroComponente', /* Nome do script */
        data() { /* Dados */
            return { /* Retornará */
                nome: "Matheus", /* Dado que irá retornar no script "nome" */
                profissao: "Programador" /* Dado que irá retornar no script "profissao" */
            }
        }
    }
</script>