<template>
    <div>
        <h1>Meu nome é: {{ nome }}</h1>  
    </div>
</template>

<script>
export default {
    name: 'LifeCycle',
    data() {
        return {
            nome: 'ainda não sei'
        }
    },
    created() {
        setTimeout(() =>{
            this.nome = 'Matheus'
        },1000);   
    },
    mounted() {
        setTimeout(() =>{
            this.nome = 'Marco'
        },2000);  
        this.lifeCycle()  
    },
    methods: {
        lifeCycle(){
            console.log('executou')
        }
    },
}
</script>