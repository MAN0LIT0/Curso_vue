<template>
<div>
  <Header />
  <componente1/>
  <p>o dado de app é: {{ teste }}</p>
  <LifeCycle/>
  <Pessoa/>
  <Form/>
</div> 
</template>
<script>
import componente1 from './components/componente1.vue'
import LifeCycle from './components/LifeCycle.vue'
import Pessoa from './components/Pessoa.vue'
import Form from './components/Form.vue'
import Header from './components/header.vue'

export default {
  name: 'App',
  components: {
    componente1,
    LifeCycle,
    Pessoa,
    Form,
    Header
  }, data() {
    return {
      teste: "testando"
    }
  },
}
</script>
<style>
  body{
    background-color: #333;
    color: aliceblue;
  }
  a {
    color: red;
  }
</style>