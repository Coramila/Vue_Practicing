<template>
 <PrimeiroComponente />
 <LifeCycle/>
 <pessoa/>
 <Form/>
</template>

<script>
  import PrimeiroComponente from './components/PrimeiroComponente.vue'
  import LifeCycle from './components/LifeCycle.vue'
  import pessoa from './components/pessoa.vue'
  import Form from './components/Form.vue'
  
  export default {
    name: 'App',
    components: {
      PrimeiroComponente,
      LifeCycle,
      pessoa,
      Form
    },

  }
</script>