<template>
    <div>
        <h1>Ola vue!!!</h1>
        <reutilizacao />
        <reutilizacao />
        <reutilizacao />
        <br>
        <p>Meu nome é: {{ nome }} e trabalho como: {{ profissao }}</p>
        <multiplosEventos />
        <reutilizacao />
        <reutilizacao />
        <reutilizacao />
        <reutilizacao />
        <reutilizacao />

    </div>
</template>
<script>
import multiplosEventos from './multiplosEventos.vue'
import reutilizacao from './reutilizacao.vue'
export default {
    name: 'componente1',
    components: {
        multiplosEventos,
        reutilizacao
    },
    data() {
        return {
            nome: "Marcos",
            profissao: "programador"
        }
    },
}
</script>