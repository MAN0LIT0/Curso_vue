<template>
<div>
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
export default {
  name: 'App',
  components: {
    componente1,
    LifeCycle,
    Pessoa,
    Form
  }, data() {
    return {
      teste: "testando"
    }
  },
}
</script>