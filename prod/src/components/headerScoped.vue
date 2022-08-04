<template>
    <ul>
        <li><a href="">home</a></li>
        <li><a href="">projetos</a></li>
        <li><a href="">contato</a></li>
    </ul>
</template>

<script>
export default {
  name: 'headerScoped'
}
</script>

<style scoped>
ul{
    list-style: none;
    display: flex;
}
li{
    margin-right: 10px;
}

a{
    color: aliceblue;
    text-decoration: none;
    transition: .5s;
}
a:hover{
    color: aquamarine;
}
</style>
