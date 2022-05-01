<template>
    <div>
        <img :src="avatar" :alt="descrisao" style="max-width:100px;">
    </div>
</template>
<script>
export default {
    name: 'Picture',
    data() {
        return {
            avatar: "/img/hosmi.png",
            descrisao: "Hosmi perssoa"
        }
    },
}
</script>