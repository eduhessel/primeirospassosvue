<template> <!--HTML-->
    <div>
        <h2>Esta é a descrição da pessoa: {{ nome }} </h2> <!--Importando dados do script "nome"-->
        <Info /> <!--Componente-->
        <Form /> <!--Componente-->
    </div>
</template>

<script> /* Javascript */
    import Info from './Info.vue'; /* Importar script */
    import Form from './Form.vue'; /* Importar script */

    export default {
        name: 'Pessoa', /* Nome do script */
        components: { /* Componentes da aplicação */
            Info, /* Componente */
            Form /* Componente */
        },
        data() { /* Dados */
            return { /* Retornará */
                nome: 'Matheus' /* Dado que irá retornar no script "nome" */
            }
        }
    }
</script>