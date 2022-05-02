<template>
    <div>
        <button @click="primeiro(txt1, $event), segundo(txt2, $event), terceiro($event)">Ativar Multiplos Eventos</button>
        <p>{{ multiplosEventos }}</p>
    </div>
</template>
<script>
export default {
    name: 'multiplosEventos',
    data() {
        return {
            multiplosEventos: "",
            txt1: "Primeiro argumento",
            txt2: "segundo argumento"

        }
    },
    methods: {
        primeiro(txt,e) {
            this.multiplosEventos = txt;
        },
        segundo(txt,e) {
            setTimeout(() => this.multiplosEventos = txt, 1000)
        },
        terceiro(e) {
            setTimeout(() => this.multiplosEventos = "", 2000)
        }
    },
}
</script>
<style scoped>
    div {
        margin: 100px;
    }
</style>