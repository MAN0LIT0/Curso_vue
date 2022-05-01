<template>
    <div>
        <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
        <p v-else>Não estou trabalhando no momento!</p>
        <p>Utiliso as seguintes tecnolias</p>
        <ul>
            <li>JavaScript</li>
            <li>PHP</li>
            <li>Python</li>
            <li>Vue</li>
        </ul>
        <Picture />
        <p v-show="mostrar_email">Mande uma mensagem para: {{ email }}</p>
        <p>Para acessar meu portifólio <a v-bind:href="meu_link" target="_blank">basta clicar aqui</a></p>
    </div>
</template>
<script>
import Picture from './Picture.vue'
export default {
    name: 'info',
    components: {
        Picture
    },
    data() {
        return {
            esta_trabalhando: true,
            mostrar_email: true,
            email: 'marcopirocadepano@gmail.com',
            meu_link: 'https://google.com'
        }
    },
}
</script>