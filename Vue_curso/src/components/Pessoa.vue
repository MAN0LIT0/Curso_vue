<template>
    <div>
        <h2>Está é a descrição de uma pessoa: {{ nome }}</h2>
        <info :email="email" :esta_trabalhando=true />
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
            nome: 'Marco',
            email: 'marcodelicinha@gmail.com'
        }
    },
}
</script>