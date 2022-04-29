<template>
    <div>
        <h2>Está é a descrição de uma pessoa: {{ nome }}</h2>
        <p>Estou trabalhando no momento.</p>
        <info />
    </div>
</template>

<script>
import info from './info.vue'
export default {
    name: 'Pessoa',
    components: {
        info
    },
    data() {
        return {
            nome: 'Marco'
        }
    },
}
</script>