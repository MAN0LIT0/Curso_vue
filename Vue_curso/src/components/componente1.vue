<template>
    <div>
        <h1>Ola vue!!!</h1>
        <br>
        <p>Meu nome é: {{ nome }} e trabalho como: {{ profissao }}</p>
        <multiplosEventos />
    </div>
</template>
<script>
import multiplosEventos from './multiplosEventos.vue'

export default {
    name: 'componente1',
    components: {
        multiplosEventos
    },
    data() {
        return {
            nome: "Marcos",
            profissao: "programador"
        }
    },
}
</script>