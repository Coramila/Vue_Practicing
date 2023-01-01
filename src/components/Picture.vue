<template>
    <img :src="avatar" alt="descricao">
</template>

<script>
export default{
    name: 'Picture',
    data(){
        return{
            avatar: "/img/perfil.JPG",
            decricao: "Camila Carvalho"
        }
    }

}
</script>