<template>
    <div>
        <img :src="avatar" :alt="descrisao" style="max-width:100px;">
        <mudarImagem @mudar-imagem="trocarImagem"/>
    </div>
</template>
<script>
import reutilizacao from './reutilizacao.vue'
import mudarImagem from './mudarIMG.vue'
export default {
    name: 'Picture',
    components: { 
        reutilizacao,
        mudarImagem
     },
    data() {
        return {
            avatar: "/img/hosmi.png",
            descrisao: "Hosmi perssoa"
        }
    },
    methods: {
        trocarImagem() {
           this.avatar = '/img/icon.png'
        }    
    },
}
</script>