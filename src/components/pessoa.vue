<template>
    <div>
        <h2>Essa é a descrição da pessoa: {{ nome }}</h2>
        <Info :email="email"/> <!-- O "email" que está em data() vai ser enviado via props para o compomente info -->
    </div>
</template>
<script>
import Info from './Info.vue'
export default {
    name: 'pessoa',
    components: {
        Info
    },
    data(){
        return{
            nome: 'Camila',
            email:"camilaa@email.com"
        }
    }

}
</script>