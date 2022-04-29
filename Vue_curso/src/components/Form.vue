<template>
    <div>
        <h1>Meu Form</h1>
        <form action="">
            <div>
                <inputText />
            </div>
            <div>
                <inputText />
            </div>
            <div>
                <submit />
            </div>
        </form>
    </div>
</template>
<script>
import inputText from './Form/inputText.vue'
import submit from './Form/submit.vue'

export default {
    name: 'Form',
    components: {
        inputText,
        submit
    }
}
</script>