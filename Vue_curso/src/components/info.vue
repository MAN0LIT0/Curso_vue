<template>
    <div>
        <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
        <p v-else>Não estou trabalhando no momento!</p>
        <p>Utiliso as seguintes tecnolias para back-end</p>
        <ul>
            <li v-for="(technology, index) in backend_technologies" v-bind:key="index">
                {{ technology }}
            </li>
        </ul>
        <p>Utilizo as seguintes tecnologias para front-end</p>
        <ul>
            <li v-for="technology in frontend_technologies" :key="technology.id">
                {{ technology.language }}
            </li>
        </ul>
        <div>
            <button @click="showEmail">{{ mostrar_botao }}</button>
        </div>
        <Picture />
        <p v-show="mostrar_email">Mande uma mensagem para: {{ email }}</p>
        <p>Para acessar meu portifólio 
            <a v-bind:href="meu_link" target="_blank">basta clicar aqui</a>
        </p>
    </div>
</template>
<script>
import Picture from './Picture.vue'
export default {
    name: 'info',
    components: {
        Picture
    },
    props: {
        email: String,
        esta_trabalhando: Boolean
    },
    data() {
        return {
            mostrar_email: false,
            meu_link: 'https://google.com',
            mostrar_botao: 'Mostrar E-mail',
            backend_technologies: ['JavaScript','PHP','Python'],
            frontend_technologies: [
                {id:1, language: 'HTML'},
                {id:3, language: 'CSS'},
                {id:2, language: 'Vue'},
            ] 
        }
    },
    methods: {
        showEmail(){
            this.mostrar_email = !this.mostrar_email
            if(!this.mostrar_email){
                this.mostrar_botao = 'Mostrar E-mail'
            }else{
                this.mostrar_botao = 'Esconder E-mail'
            }
        }    
    },
}
</script>