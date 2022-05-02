<template>
    <div>
        <h1>Meu Form</h1>
        <form action="" @submit="enviarFormulario($event)">
            <div>
                <input type="" v-model="name">
            </div>
            <div>
                <input type="" v-model="email">
            </div>
            <div>
                <submit />
            </div>
        </form>
    </div>
</template>
<script>
import inputText from './Form/inputText.vue'
import submit from './Form/submit.vue'

export default {
    name: 'Form',
    components: {
        inputText,
        submit
    },
    data() {
        return {
            name: "",
            email: ""
        }
    },
    methods: {
        enviarFormulario(e) {
            e.preventDefault();
            
            const name = this.name;
            const email = this.email;
            console.log('O nome é: ' + name);
            console.log('O email é: ' + email);

            // ajax

            // inserir no banco de dados
        }
    },
}
</script>