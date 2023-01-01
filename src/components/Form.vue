<template>
    <div>
        <h2>Meu formulário</h2>
    <form action="" @submit="enviarFormulario($event)">
        <div>
            <input v-model="nome">
        </div>
        <div>
            <input v-model="email">
        </div>
        <div>
            <Submit/>
        </div>
    </form>
</div>
</template>

<script>
import InputText from './Form/InputText.vue';
import Submit from './Form/Submit.vue';

export default{
    name: 'Form',
    components:{
        InputText,
        Submit
    },
    data(){
        return{
            nome:"",
            email:""
        }
    },
    methods:{
        enviarFormulario(e){ // O 'e' está relacionado ao '$event' do form, e nos permite acessar a função preventDefault
            e.preventDefault(); //Previde que ao submeter o formulário a página seja recarregada
            
            const nome = this.nome;
            const email = this.email;
                       
            console.log("Enviado!");
            console.log("Nome: " + nome);
            console.log("Email: " + email);

        }
    }
}

</script>