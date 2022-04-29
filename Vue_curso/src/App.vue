<template>
<div>
  <componente1/>
  <p>o dado de app é: {{ teste }}</p>
</div> 
</template>
<script>
import componente1 from './components/componente1.vue'
export default {
  name: 'App',
  components: {
    componente1
  }, data() {
    return {
      teste: "testando"
    }
  },
}
</script>