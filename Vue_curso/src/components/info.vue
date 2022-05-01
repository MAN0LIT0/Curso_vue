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
        <p v-show="mostrar_email">Mande uma mensagem para: {{ email }}</p>
    </div>
</template>
<script>
export default {
    name: 'info',
    data() {
        return {
            esta_trabalhando: true,
            mostrar_email: true,
            email: 'marcopirocadepano@gmail.com'
        }
    },
}
</script>