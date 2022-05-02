<template>
    <div>
        <img :src="avatar" :alt="descrisao" style="max-width:100px;">
        <reutilizacao />
    </div>
</template>
<script>
import reutilizacao from './reutilizacao.vue'
export default {
  components: { reutilizacao },
    name: 'Picture',
    data() {
        return {
            avatar: "/img/hosmi.png",
            descrisao: "Hosmi perssoa"
        }
    },
}
</script>