<template>
  <Header/>
 <PrimeiroComponente />
 <p class="paragrafo-pai">O dado de app é: {{ testando }}</p>
 <LifeCycle/>
 <pessoa/>
 <Form/>
</template>

<script>
  import PrimeiroComponente from './components/PrimeiroComponente.vue'
  import LifeCycle from './components/LifeCycle.vue'
  import pessoa from './components/pessoa.vue'
  import Form from './components/Form.vue'
  import Header from './components/Header.vue'
  
  export default {
    name: 'App',
    components: {
      Header,
      PrimeiroComponente,
      LifeCycle,
      pessoa,
      Form
    },

    data(){
      return{
        testando: "teste"
      }
    }

  }
</script>

<style>

body{
  background-color: #333;
  color: #fff;
}

a{
  color: red;
}

.teste{
  background-color: black;
}

</style>