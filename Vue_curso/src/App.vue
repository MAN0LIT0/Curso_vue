<template>
<div>
  <componente1/>
  <p>o dado de app é: {{ teste }}</p>
  <LifeCycle/>
</div> 
</template>
<script>
import componente1 from './components/componente1.vue'
import LifeCycle from './components/LifeCycle.vue'
export default {
  name: 'App',
  components: {
    componente1,
    LifeCycle
  }, data() {
    return {
      teste: "testando"
    }
  },
}
</script>