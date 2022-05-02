<template>
    <div>
        <button @click="$emit('mudarImagem')">Tocar imagem de perfil</button>
    </div>
</template>
<script>
export default {
    name: 'mudarIMG',
    emits: ['mudarimagem']
}
</script>