<template>
    <div>
        <ul>
            <li><a href="#">Link 1</a></li>
            <li><a href="#">Link 2</a></li>
            <li><a href="#">Link 3</a></li>
            <li><a href="#">Link 4</a></li>
        </ul>
    </div>
</template>
<script>
export default {
    name: 'header'
}
</script>
<style scoped>
    ul {
        list-style: none;
        display: flex;
        background-color: #c9c9;
    }

    li {
        padding: 5px;
        margin-right: 20px;
        background-color: aqua;
        border-radius: 10px;
        font-weight: bold;
        transition: .5s;   
    }

    a {
        color: blueviolet;
        text-decoration: none;
        transition: .5s;  
    }
    a:hover{
        color: coral;
    }
    li:hover{
        background-color: rgb(83, 189, 101);
    }
</style>