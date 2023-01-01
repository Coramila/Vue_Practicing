<template>
    <img :src="avatar" alt="descricao">
    <MudarImagem @mudar-imagem="trocarImagem" /> <!--A emissão do método que foi resgatado por @mudar-imagem (que é o emit) ativa o método trocarImagem, que é o método do meu componente atual-->
</template>

<script>
import MudarImagem from './MudarImagem.vue';

export default{
    name: "Picture",
    components: { MudarImagem },
    data() {
        return {
            avatar: "/img/perfil.JPG",
            decricao: "Camila Carvalho"
        };
    },
    methods:{
        trocarImagem(){
            this.avatar='/img/perfil2.jpg'
        }
    }    
}
</script>