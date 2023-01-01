<template>
    <div>
        <h1>Olá Vue!</h1>
        <p>Meu nome é {{ nome }} e trabalho como {{ profissao }}</p>
        <MultiplosEventos/>
        <Reutilicacao/>
        <Reutilicacao/>
        <Reutilicacao/>
        <Reutilicacao/>
    </div>
</template>

<script>
import MultiplosEventos from './MultiplosEventos.vue'
import Reutilicacao from './Reutilicacao.vue';
    export default{
        name:'PimeiroComponente',
        components:{
            MultiplosEventos,
            Reutilicacao
        },
        data(){
            return {
                nome: "Camila",
                profissao: "Programadora"
            }
        }
    }

</script>