<template> <!--HTML-->
    <form action="">
        <div>
            <InputText /> <!--Componente-->
        </div>

        <div>
            <InputText /> <!--Componente-->
        </div>

        <div>
            <Submit /> <!--Componente-->
        </div>
    </form>
</template>

<script> /* Javascript */
    import InputText from './form/InputText.vue' /* Importar script */
    import Submit from './form/Submit.vue' /* Importar script */

    export default {
        name: 'Form', /* Nome do script */
        components: { /* Componentes da aplicação */
            InputText, /* Componente */
            Submit /* Componente */
        }
    }
</script>