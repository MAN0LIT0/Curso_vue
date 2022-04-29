<template>
    <div>
        <h1>Ola vue!!!</h1>
        <br>
        <p>Meu nome é: {{ nome }} e trabalho como: {{ profissao }}</p>
    </div>
</template>
<script>
export default {
    name: 'componente1',
    data() {
        return {
            nome: "Marcos",
            profissao: "programador"
        }
    },
}
</script>